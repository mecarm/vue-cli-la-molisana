<template>
    <div class="card">
        <img :src="dettagliLinea.img" alt="">
        <h3>{{dettagliLinea.name}}</h3>
    </div>
</template>

<script>
export default {
    name: 'LineaComp',
    props: {
        dettagliLinea: Object
    }
}
</script>

<style lang="scss" scoped>
.card {
    width: calc((100% / 3) - 20px);
    text-align: center;
    border: 1px solid rgb(198, 196, 196);
    margin: 10px;
    padding: 20px;

    img {
        width: 100%;
    }
}
</style>