<template>
    <footer class="text-center mt-5">
        <h6 class="fs-4 mt-2 pt-4">Vuoi organizzare una festa? Contattaci</h6>
        <div class="container">
            <form action="" class="form-group">
                <input class="form-control mt-2" type="number" placeholder="Inserisci un numero di telefono per essere contattato">
                <textarea class="form-control mt-2" type="text" placeholder="Inviaci un messaggio"></textarea>
                <input type="submit" class="mt-2 btn btn-primary">
            </form>
        </div>  
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