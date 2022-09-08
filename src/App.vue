<template>
  <Header></Header>
  <Info />
  <Generator />
  <Footer></Footer>
</template>

<script>
import Header from './components/header.vue'
import Info from './components/info.vue'
import Generator from './components/generator.vue'
import Footer from './components/footer.vue'

export default {
  name: 'App',
  components: {
    Header, Info, Generator, Footer
  }
}
</script>

<style>

</style>
