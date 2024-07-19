<template>
    <div id="lmf-slider">
        <div class="lmf-slider-container">
            <img v-for="(image, index) in images" :key="index" :src="image" :alt="'Image ' + (index + 1)" :class="{ active: index === currentImageIndex }">
        </div>
    </div>
</template>

<script>
export default {
    name: 'SliderComponent',
    data() {
        return {
            images: [
                "/1.jpg",
                "/2.jpg",
                "/3.jpg",
                "/4.jpg",
            ],
            currentImageIndex: 0
        }
    },
    mounted() {
        this.startSlideshow();
    },
    methods: {
        startSlideshow() {
            setInterval(() => {
                this.currentImageIndex = (this.currentImageIndex + 1) % this.images.length;
            }, 4000); 
        }
    }
}
</script>

<style lang="scss" scoped>
#lmf-slider {
    width: 100%;
    height: 1000px;
    overflow: hidden;
    position: relative;
}

.lmf-slider-container {
    position: relative;
    width: 100%;
    height: 100%;
}

.lmf-slider-container img {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 600px;
    object-fit: cover;
    opacity: 0;
    transition: opacity 1s ease-in-out;
}

.lmf-slider-container img.active {
    opacity: 1;
}
</style>