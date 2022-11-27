<template>
  <div class="container">
    <div class="card">
        <div>
            <i class="fa-solid fa-plate-wheat"></i>
        </div>
        <h1>Il Grano</h1>
        <p>UTILIZZIAMO SOLO GRANO COLTIVATO IN MOLISE, ABRUZZO, PUGLIA, LAZIO E MARCHE, REGIONI DA SEMPRE VOCATE ALLA PRODUZIONE DI GRANO DURO DI ALTA QUALITÀ.</p>
    </div>
    <div class="card">
        <div>
            <i class="fa-solid fa-stapler"></i>
        </div>
        <h1>Il Molino</h1>
        <p>MACINIAMO DA CINQUE GENERAZIONI IL MIGLIOR GRANO, LO DECORTICHIAMO A PIETRA PER PRODURRE SEMOLE PIÙ SICURE DAL PUNTO DI VISTA IGIENICO-SANITARIO.</p>
    </div>
    <div class="card">
        <div>
            <i class="fa-solid fa-industry"></i>
        </div>
        <h1>Il Pastificio</h1>
        <p>TRAFILIAMO AL BRONZO PER OTTENERE UNA PASTA RUVIDA E TENACE CON UN’ECCELLENTE TENUTA IN COTTURA.</p>
    </div>
    <div class="card">
        <div>
            <i class="fa-solid fa-droplet"></i>
        </div>
        <h1>L'Acqua</h1>
        <p>IMPASTIAMO LE NOSTRE SEMOLE CON ACQUA PURA, IPOSODICA CON CARATTERISTICHE OLIGOMINERALI DELLE SORGENTI DEL MATESE.</p>
    </div>
  </div>
</template>

<script>
export default {
    name: 'BrandSection'
}
</script>

<style lang="scss" scoped>
.container{
    width: 90%;
    margin: 20px auto;
    display: flex;
    justify-content: space-between;

    .card{
        width: calc(100% / 5);
        text-align: center;
        color: #483012;

        h1{
            margin: 5px 0;
        }
        p{
            text-align: center;
            font-size: 0.8rem;
        }

        div{
            margin: 5px 0;
            background: #483012;
            color: white;
            display:  inline-block;
            padding: 25px;
            border-radius: 50%;

            i{
                font-size: 2.0rem;
            }
        }
    }
}
</style>