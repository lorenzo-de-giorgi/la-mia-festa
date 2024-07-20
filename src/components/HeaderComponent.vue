<template>
    <nav>
        <div class="container d-flex justify-content-between align-items-center">
            <div>
                <img id="lmf-logo" src="/logo.jpg">
            </div>
            <div id="lmf-nav">
                <ul class="d-flex me-2">
                    <li class="me-4 list-unstyled no-wrap" v-for="navItem in Items" :key="navItem.id">
                        <a id="lmf-nav-link" :href="navItem.link">{{ navItem.name }}</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
    <SliderComponent />
</template>

<script>
import SliderComponent from './SliderComponent.vue';

    export default {
        name: 'HeaderComponent',
        components: {
            SliderComponent,
        },
        data() {
            return {
                Items: [
                    { id: 1, name: 'Chi Siamo', link: '/about' },
                    { id: 2, name: 'Contattaci', link: '/contacts' },
                    { id: 3, name: 'Immagini', link: '/image' },
                ]
            }
        },
    }
</script>

<style lang="scss" scoped>
    @use '../assets/styles/partials/variables' as *;

    #lmf-logo{
        width: 30%;
    }

    #lmf-nav-link{
        text-decoration: none;
        color: $gold;
        font-size: 15px;
    }

    .no-wrap {
        white-space: nowrap;
    }
</style>