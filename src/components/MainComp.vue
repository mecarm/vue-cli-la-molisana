<template>
  <div>
    <div class="prodotti">
        <h1>SCOPRI TUTTI I <strong>PRODOTTI</strong></h1>
        <h2>Scopri la <strong>pasta La Molisana:</strong> tipi e formati di pasta da grano 100% italiano decorticato a pietra e trafilata al bronzo.</h2>
    </div>
    <div class="pre-pasta">
        <i class="fa-solid fa-vector-square"></i>
        <span>Pasta per <strong>forma</strong></span>
    </div>
    <div class="cards">
        <PastaCard v-for="(element, index) in pasta" :key="index" :dettagliPasta="element"/>
    </div>
    <div class="pre-pasta">
        <i class="fa-solid fa-vector-square"></i>
        <span>Pasta per <strong>linea</strong></span>
    </div>
    <div class="cards">
        <LineaComp v-for="(element, index) in linea" :key="index" :dettagliLinea="element"/>
    </div>
  </div>
</template>

<script>
import PastaCard from './PastaCard.vue'
import LineaComp from './LineaComp.vue'

export default {
    name: 'MainComp',
    components: {
        PastaCard,
        LineaComp
    },
    data() {
        return {
            pasta: [
                {
                    "img": "https://www.lamolisana.it/wp-content/uploads/2021/03/1-spaghetto-quadrato-2.png",
                    'tipo': 'Pasta Lunga'
                },
                {
                    "img": "https://www.lamolisana.it/wp-content/uploads/2021/05/29-caserecce-molisane.png",
                    'tipo': 'Pasta Corta'
                },
                {
                    "img": "https://www.lamolisana.it/wp-content/uploads/2021/03/15-spaghetti-1.png",
                    'tipo': 'Spaghetti'
                },
                {
                    "img": "https://www.lamolisana.it/wp-content/uploads/2021/05/20-penne-rigate.png",
                    'tipo': 'Penne'
                },
                {
                    "img": "https://www.lamolisana.it/wp-content/uploads/2022/01/28-fusilli.png",
                    'tipo': 'Fusilli'
                },
                {
                    "img": "https://www.lamolisana.it/wp-content/uploads/2021/05/ziti-tagliati.webp",
                    'tipo': 'Ziti'
                },
                {
                    "img": "https://www.lamolisana.it/wp-content/uploads/2021/10/gnocchi.png",
                    'tipo': 'Gnocchi'
                },
                {
                    "img": "https://www.lamolisana.it/wp-content/uploads/2021/10/50-ditalini-rigati-grandi-cucine.png",
                    'tipo': 'Ditali'
                },
                {
                    "img": "https://www.lamolisana.it/wp-content/uploads/2022/04/pastina.webp",
                    'tipo': 'Pastina'
                },
            ],
            linea: [
                {
                    'img': "https://www.lamolisana.it/wp-content/uploads/2022/04/pasta-classica.webp",
                    'name': "Le classiche"
                },
                {
                    'img': "https://www.lamolisana.it/wp-content/uploads/2021/06/32-mezzi-rigatoni-integrali.webp",
                    'name': "Le integrali"
                },
                {
                    'img': "https://www.lamolisana.it/wp-content/uploads/2022/04/pasta-speciale.webp",
                    'name': "Le speciali"
                },
                {
                    'img': "https://www.lamolisana.it/wp-content/uploads/2022/04/pasta-biologica.webp",
                    'name': "Le biologiche"
                },
                {
                    'img': "https://www.lamolisana.it/wp-content/uploads/2022/08/pasta-sfiziosa.webp",
                    'name': "Le sfiziose"
                },
                {
                    'img': "https://www.lamolisana.it/wp-content/uploads/2022/04/pasta-senza-glutine.webp",
                    'name': "Gluten-free"
                },
                {
                    'img': "https://www.lamolisana.it/wp-content/uploads/2022/04/le-semole.webp",
                    'name': "Le semole"
                },
                {
                    'img': "https://www.lamolisana.it/wp-content/uploads/2022/04/rossi.webp",
                    'name': "I Rossi"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.prodotti {
    width: 80%;
    margin: 5px auto;
    display: flex;
    justify-content: space-between;

    h1{
        flex-basis: 50%;
        font-weight: normal;
        padding-top: 20px;

    }
    h2{
        flex-basis: 50%;
        font-style: italic;
        font-weight: normal;
        background: rgb(246, 238, 238);
        padding: 10px;
    }
}
.pre-pasta{

    margin: 30px auto;
    width: 80%;
    font-size: 1.8rem;
    font-style: italic;

    span{
        padding-left: 10px;
    }
}

.cards{
    margin:10px auto;
    width: 80%;
    display: flex;
    flex-wrap: wrap;
}
</style>