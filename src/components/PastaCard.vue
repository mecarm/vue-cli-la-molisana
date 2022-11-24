<template>
    <div class="card">
        <img :src="dettagliPasta.img" alt="">
        <h3>{{dettagliPasta.tipo}}</h3>
    </div>
</template>
  

<script>
export default {
    name: 'PastaCard',
    props: {
        dettagliPasta: Object
    }
}
</script>

<style lang="scss" scoped>
    .card{
        width: calc((100% / 5) - 20px);
        text-align: center;
        border: 1px solid rgb(198, 196, 196);
        margin: 10px;
        padding: 20px;

        img{
            width: 100%;
        }
    }
</style>

