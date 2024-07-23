<template>
  <HeaderComponent />
  <MainComponent />
  <LeftImageComponent />
  <RightImageComponent />
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import LeftImageComponent from './components/LeftImageComponent.vue';
import RightImageComponent from './components/RightImageComponent.vue';
  export default {
    name: 'App',
    components: {
      HeaderComponent,
      MainComponent,
      LeftImageComponent,
      RightImageComponent
    }
    
  }
</script>

<style lang="scss" scoped>

</style>