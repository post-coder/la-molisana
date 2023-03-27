<script>

export default {
  name: "AppPasta",
  data() {


  },

  // per definire le prop dobbiamo inserirle nell'oggetto "props"
  // indicando il loro nome e il loro tipo
  props: {
    // nome: Tipo
    // stiamo attenti che il tipo deve iniziare con la lettera maiuscola
    // ricordiamoci che sono "read-only", non sono modificabili in nessun modo (da dentro il component)
    img: String,
    title: String,
  },

}

</script>

<template>
  <div class="pasta">
    <img :src="img" alt="">
    <!-- le prop vengono interpolate e chiamate come delle semplici proprietà in data() -->
    <div class="title">{{title}}</div>
  </div>
</template>

<style lang="scss">
  .pasta {
    width: 200px;
    background-color: white;
    border: 1px solid #dce8fd;

    padding: 12px;

    color: darkblue;

    font-weight: bold;

    img {
      width: 100%;
    }
  }
</style>