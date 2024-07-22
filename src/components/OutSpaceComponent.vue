<template>
    <div class="container">
        <div class="card">
            <img id="lmf-img-esterno" src="/public/esterno.jpg" alt="Immagine Esterno Locale">
            <p class="heading">Spazio Esterno</p>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'OutSpaceComponent'
    }
</script>

<style lang="scss" scoped>
    @use '../assets/styles/partials/variables' as *;

    .card {
        position: relative;
        width: 50%;
        height: 100%;
        background-color: $gold;
        display: flex;
        flex-direction: column;
        justify-content: end;
        padding: 12px;
        gap: 12px;
        border-radius: 8px;
        cursor: pointer;
        color: white;
        overflow: hidden;
    }

    #lmf-img-esterno{
        width: 100%;
        transform: translate(-50% -50%) ;
        border-radius: 8px;
    }

    .heading {
        font-size: 20px;
        text-transform: capitalize;
        font-weight: 700;
        position: absolute;
        color: black;
        margin-left: 10px;
    }

    .card p:not(.heading) {
        font-size: 14px;
    }
</style>