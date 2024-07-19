<template>
  <HeaderComponent />
  <SliderComponent />
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import SliderComponent from './components/SliderComponent.vue';
  export default {
    name: 'App',
    components: {
      HeaderComponent,
      SliderComponent
    }
    
  }
</script>

<style lang="scss" scoped>

</style>