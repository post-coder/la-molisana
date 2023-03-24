<script>
  import AppHeader from "./components/AppHeader.vue";
  import AppMain from "./components/AppMain.vue";
  import AppFooter from "./components/AppFooter.vue";

  export default {
    data() {
      return {

      }
    },

    components:  {
      AppHeader,
      AppMain,
      AppFooter,
    }
  }
</script>

<template>
  <div>
    <AppHeader></AppHeader>

    <AppMain></AppMain>

    <div class="container">
      
      <div class="row row-cols-2">
        <div class="col">colonna</div>
        <div class="col">colonna</div>
        <div class="col">colonna</div>
      </div>

      <i class="fas fa-search"></i>


    </div>
    
    <AppFooter></AppFooter>
  </div>
</template>


<style lang="scss" scoped>



</style>