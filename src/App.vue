<script>
  import Header from "./components/AppHeader.vue"
  import Jumbo from "./components/AppJumbo.vue"
  import Footer from "./components/AppFooter.vue"

   export default {
    data() {
      return {

      }
    },

    components: {
      Header,
      Jumbo,
      Footer,
    }
   }
</script>

<template>
  <div>
    <Header></Header>

    <Jumbo></Jumbo>

    <Footer></Footer>
  </div>
</template>

<style scoped>

</style>
