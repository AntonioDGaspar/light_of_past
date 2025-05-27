<template>
    <div id="banner">
        <p> Conheça os Mistérios esquecidos pela Humanidade </p>
    </div>
</template>

<script>
    export default {
        name: "banner"
    }
</script>

<style scoped>
    #banner {
        background-image: url("@/../public/img/Fundo.jpg");
        background-size: cover;
        display: flex;
        align-items: center;
        width: 100vw;
        height: 670px;
        box-shadow: 0px 3px 10px rgba(0, 0, 0, 0.705);
    }

    #banner p {
        font-size: 3em;
        color: var(--cor02);
        width: 500px;
        margin-left: 30px;
        padding: 5px 5px 5px 10px;
        background-color: #222222d7;
        border-radius: 10px;
        font-size: 2.7em;
    }
</style>