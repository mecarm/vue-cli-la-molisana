<template>
  <header>
    <div class="logo">
      <img alt="Logo La Molisana" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRnZqUiuz3n_xv29KpY8sv-Pn2kvQyENIjRU7_cilw&s">
      <div>
        <i class="fa-solid fa-magnifying-glass"></i>
        <select>
          <option value="">Italia</option>
        </select>
        <span class="menu">
          <span>MENU</span>
          <i class="fa-solid fa-bars"></i>
        </span>
      </div>
    </div>
    <div class="line">
      <div class="home">
        <i class="fa-solid fa-house-chimney"></i>
      </div>
      <button>CATALOGO PRODOTTI</button>
      <hr>
    </div>
  </header>
</template>

<script>
export default {
  name: 'HeaderComp',
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .logo{
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;

    div{
      position: absolute;
      right: 200px;
      display: flex;
      align-items: center;

      select{
        padding: 5px 20px;
        margin-left: 20px;
      }

      .menu{
        display: flex;
        align-items: center;
        margin-left: 20px;
        color: #BC1C1C; 

        span{
          margin-right: 5px;
          font-size: 0.8rem;
          font-weight: bold;
        }
      }
    }
    i{
      font-size: 1.4rem;
    }
  }

  .line{
    width: 80%;
    margin: auto;

    .home{
      background: #BC1C1C;
      color: white;
      display: inline-block;
      padding: 8px 10px;
      border-radius: 50%;
    }

    button{
      margin-left: 10px;
      padding: 10px;
      border: none;
      background: #ECECEC;
      font-weight: bold;
    }

    hr{
      border: 1px solid black;
    }
  }
</style>
