<template>
    <div>
        <div class="line-divisor">
            <div class="line">
            </div>
            <div class="logo">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRnZqUiuz3n_xv29KpY8sv-Pn2kvQyENIjRU7_cilw&s" alt="logo">
            </div>
            <div class="line">
            </div>
        </div>
        <div class="container">
            <div>
                <ul>
                    <h4>LA NOSTRA PASTA</h4>
                    <li>Pasta Classica</li>
                    <li>Pasta Integrale</li>
                    <li>Pasta Biologica</li>
                    <li>Pasta Senza Glutine</li>
                    <li>Pasta Lunga</li>
                    <li>Pasta Corta</li>
                    <li>Pastina</li>
                    <li>Gnocchi</li>
                    <li>Spaghetti</li>
                    <li>Penne</li>
                    <li>Fusilli</li>
                    <li>Ziti</li>
                    <li>Ditali</li>
                </ul>
            </div>
            <div>
                <ul>
                    <h4>LE NOSTRE RICETTE</h4>
                    <li>Tutte le ricette</li>
                    <li>Ricette con Gnocchi</li>
                    <li>Ricette di pasta semplici e veloci</li>
                    <li>Ricette di pasta fredda</li>
                    <li>Ricette con Orecchiette</li>
                    <li>Ricette con Lasagne </li>
                    <li>Ricette con Tagliatelle</li>
                    <li>Ricette con Cannelloni</li>
                    <li>Ricette con Paccheri</li>
                    <li>Ricette con Spaghetti</li>
                    <li>Ricette di pasta estive</li>
                </ul>
            </div>
            <div>
                <ul>
                    <h4>IL NOSTRO BLOG</h4>
                    <li>Tutti gli articoli</li>
                    <li>Blog Cucina</li>
                    <li>Blog Nutrizione</li>
                    <li>Blog Info e notizie</li>
                </ul>
            </div>
            <div>
                <ul>
                    <h4>SERVIZI</h4>
                    <li>E-commerce</li>
                    <li>B2B</li>
                    <li>Contatti</li>
                    <li>Lavora con noi</li>
                    <li>Certificazioni</li>
                    <li>Dati aziendali</li>
                </ul>
            </div>
        </div>
        <div class="line"></div>
        <div>COLTIVATO</div>
    </div>
</template>

<script>
export default {
    name: 'FooterComp'
}
</script>

<style lang="scss" scoped>
.container{
        display: flex;
        justify-content: space-between;
        width: 80%;
        margin: 30px auto;
        color: #483012;

        li{
            list-style: none;
        }

        h4{
            margin: 10px 0;
        }

    }

.line-divisor {
    display: flex;
    align-items: center;

    .line{
        flex-grow: 1;
    }
    .logo{
        width: 5%;
        

        img{
            width: 100%;
        }
    }
}
.line{
    border-top: 1px solid black;
    margin: 0 20px;
}
</style>