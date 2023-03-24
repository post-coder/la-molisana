<script>
export default{
  data() {
    return {
      footerColumns: [
        {
          title: 'Pastificio',
          links: [
            'Il pastificio',
            'Grano',
            'Filiera',
            '100 anni di pasta',
            'Sartoria della pasta',
          ]
        },
        {
          title: 'Prodotti',
          links: [
            'Le classiche',
            'Le integrali',
            'Le speciali',
            'Le biologiche',
            'Le Gluten-free',
          ]
        }
      ],
    }
  }
}
</script>

<template>
  <footer>

    <div>
      <img src="/img/la-molisana-logo.png" alt="">
    </div>

    <div v-for="footerColumn in footerColumns" class="columns">
      <strong> {{ footerColumn.title  }} </strong>
      <ul>
        <li v-for="link in footerColumn.links"> {{ link }}</li>
      </ul>
    </div>
  

  </footer>
</template>

<style lang="scss" scoped>


footer {
  display: flex;
  flex-direction: row;
  justify-content: space-around;

  padding: 60px;
  padding-bottom: 140px;

  background-image: url('/img/footer-montagne-bottom.jpg');
  background-repeat: no-repeat;
  background-position: bottom;

  .columns {
    display: flex;
    flex-direction: column;

    strong {
      color: darkblue;
      text-transform: uppercase;

      margin-bottom: 1em;
    }
  }
}

</style>