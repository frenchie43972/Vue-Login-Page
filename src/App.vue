<template>
  <Header />
  <div>
    <router-view/> 
  </div>
  <Footer />
</template>

<script>
import Header from "./components/Header-page.vue"
import Footer from "./components/Footer-page.vue"

export default {
  name: 'App',
  components: {
    Header,
    Footer,
  }
}
</script>

<style>

</style>