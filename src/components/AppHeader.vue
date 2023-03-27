<script>
export default {
  data() {
    return {
      links: [
        'Home',
        'Prodotti',
        'Chi Siamo',
        'Contatti',
      ],
    }
  }
}
</script>

<template>
  <div>
    <div id="logo">
      <!-- per accedere alle immagini dobbiamo inserirle in public/ e accedervi
      con lo / iniziale -->
      <img src="/img/la-molisana-logo.png" alt="">
    </div>
    
    <nav id="links">
      <ul>
        <li v-for="link in links"> {{ link }} </li>
      </ul>
    </nav>
    
  </div>
</template>

<style lang="scss" scoped>
  
  #logo {
  text-align: center;
  }

  #links {

    ul {
      display: flex;
      flex-flow: row nowrap;
      justify-content: center;

      li {
        padding: 12px;

        &:hover {
          background-color: #dae9fe;
        }
      }
    }
  }

</style>