<template>
  <HeaderComponent />
  <MainComponent />
  <LeftImageComponent />
  <RightImageComponent />
  <FooterComponent />
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import LeftImageComponent from './components/LeftImageComponent.vue';
import RightImageComponent from './components/RightImageComponent.vue';
import FooterComponent from './components/FooterComponent.vue';
  export default {
    name: 'App',
    components: {
      HeaderComponent,
      MainComponent,
      LeftImageComponent,
      RightImageComponent,
      FooterComponent
    }
    
  }
</script>

<style lang="scss" scoped>

</style>