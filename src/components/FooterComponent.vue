<template>
    <footer class="text-center mt-5">
        Test Footer
    </footer>
</template>

<script>
    export default {
        name: 'FooterComponent'
    }
</script>

<style lang="scss" scoped>
  @use '../assets/styles/partials/variables' as *;

    footer{
        background-color: $gold;
    }
</style>