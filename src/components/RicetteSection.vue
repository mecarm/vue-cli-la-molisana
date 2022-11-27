<template>
  <div class="container">
    <div class="card ricette">
        <h1>LE RICETTE</h1>
        <p>Tutte le nostre Ricette di Primi Piatti di Pasta La Molisana: ingredienti, preparazione, consigli e tanto altro per ricette di pasta per tutti i palati.</p>
        <div><button>APRI</button></div>
    </div>
    <div class="card blog">
        <h1>IL BLOG</h1>
        <p>Perché dopo anni di ricerca siamo fieri di annunciare che La Molisana è a scaffale con una pasta di solo grano italiano</p>
        <div><button>APRI</button></div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'RicetteSection'
}
</script>

<style lang="scss" scoped>
    .container{
        width: 90%;
        margin: 50px auto;
        display: flex;
        justify-content: space-between;
        color: white;
        .card{
            text-align: center;
            padding: 50px;
            width: calc(100% / 2);
            margin: 10px;
            aspect-ratio: 16/9;
            display: flex;
            flex-direction: column;
            justify-content: center;
            border-radius: 5px ;
            font-size: 1.2rem;
            font-weight: bold;

            &:hover{
                opacity: 0.8;
            }
        }

        div{
            margin-top: 20px;
        }

        button{
            background: rgba(255, 255, 255, 0);
            border: 1px solid white;
            padding: 10px 30px;
            color: white;
            cursor: pointer;
        }

        .ricette{
            background-image: url('https://images.unsplash.com/photo-1579684947550-22e945225d9a?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1674&q=80');
            background-position: center;
            background-size: cover;
            background-repeat: no-repeat;

        }
        .blog{
            background-image: url('https://images.unsplash.com/photo-1515276427842-f85802d514a2?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1776&q=80');
            background-position: center;
            background-size: cover;
            background-repeat: no-repeat;
        }
    }
</style>