<template>
    <div class="container d-flex justify-content-between align-items-center">
        <div class="lmf-out-space-text text-center">
            <h4>Il nostro Spazio Interno</h4>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur, magni iusto inventore quasi excepturi dolor modi. Quis nesciunt deleniti dolorum autem. Eum vero sapiente ea harum! Nemo, sit. Excepturi voluptatem, est dolorem id aperiam consectetur? Voluptas repudiandae inventore culpa expedita omnis! Corrupti, dolorem, odit adipisci amet debitis esse tempore ipsum velit hic maiores dolores modi consequuntur nihil animi rerum ad laborum porro quos itaque asperiores at qui. Pariatur commodi eaque omnis nisi, quas fuga impedit vero delectus, natus numquam laboriosam ullam hic sed quam est ipsam recusandae officia fugit. Officia, harum odit sunt vitae est nihil beatae quas magni ratione nemo, delectus illo nostrum fuga consequatur temporibus consequuntur eum tempore voluptatum enim reprehenderit facilis voluptates non voluptatem. Eaque a repellat pariatur expedita. Praesentium, quis exercitationem. Nulla, delectus culpa at iusto corporis fugit. Quaerat pariatur illo nesciunt delectus quis, velit repellendus ipsa explicabo cum rem fugit harum laborum dolorum ducimus excepturi voluptatibus itaque animi dicta? Amet, quam laborum quo debitis esse nihil nesciunt veniam ratione rem explicabo id soluta recusandae accusamus excepturi corrupti. Voluptas nostrum amet ullam odit temporibus earum, enim neque? Delectus impedit quos nemo magni ut, minima ab repellendus vitae? Illo a reiciendis est ipsum consectetur laboriosam, tenetur vel.</p>
        </div>
        <div class="card">
            <img id="lmf-img-esterno" src="/esterno.jpg" alt="Immagine Esterno Locale">
            <p class="heading">Spazio Interno</p>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'RightImageComponent'
    }
</script>

<style lang="scss" scoped>
    @use '../assets/styles/partials/variables' as *;

    .container {
        margin-top: 100px;
        display: flex;
        align-items: center;
        gap: 20px; // Aggiungi un po' di spazio tra l'immagine e il testo
    }

    .card {
        position: relative;
        width: 50%;
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

    #lmf-img-esterno {
        width: 100%;
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

    .lmf-out-space-text {
        width: 50%; // Assicura che il testo occupi l'altra metà della larghezza del contenitore
    }
</style>