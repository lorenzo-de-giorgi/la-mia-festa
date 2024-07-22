<template>
  <HeaderComponent />
  <MainComponent />
  <OutSpaceComponent />
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import OutSpaceComponent from './components/OutSpaceComponent.vue';
  export default {
    name: 'App',
    components: {
      HeaderComponent,
      MainComponent,
      OutSpaceComponent
    }
    
  }
</script>

<style lang="scss" scoped>

</style>