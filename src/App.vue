<template>
  <HeaderComponent />
  <MainComponent />
  <LeftImageComponent />
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import LeftImageComponent from './components/LeftImageComponent.vue';
  export default {
    name: 'App',
    components: {
      HeaderComponent,
      MainComponent,
      LeftImageComponent
    }
    
  }
</script>

<style lang="scss" scoped>

</style>