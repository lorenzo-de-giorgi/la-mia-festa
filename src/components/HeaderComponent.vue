<template>
    <nav class="d-flex justify-content-between align-items-center">
        <div>
            <img id="lmf-logo" src="/logo.jpg">
        </div>
        <div id="lmf-nav">
            <ul class="d-flex me-4">
                <li class="me-4 list-unstyled" v-for="navItem in Items" :key="navItem.id">
                    <a id="lmf-nav-link" :href="navItem.link">{{ navItem.name }}</a>
                </li>
            </ul>
        </div>
    </nav>
</template>

<script>
    export default {
        name: 'HeaderComponent',
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
    }

</style>