<template>
  <div id="app">
    <Header />
    <Carousel />
    <Cards />
    <div class="container">
      <div class="row mb-5">
        <Sidebar />
        <Content />
      </div>
    </div>
    <Footer />    
    <CarouselModal />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Carousel from './components/Carousel.vue'
import Cards from './components/Cards.vue'
import Sidebar from './components/Sidebar.vue'
import Content from './components/Content.vue'
import Footer from './components/Footer.vue'
import CarouselModal from './components/CarouselModal.vue'

export default {
  name: 'App',
  components: {
    Header,
    Carousel,
    Cards,
    Sidebar,
    Content,
    Footer,
    CarouselModal
  },
  data() {
    return {

    }
  }
}

</script>

<style lang="scss">

</style>
