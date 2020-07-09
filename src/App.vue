<template>
  <div id="app">
    <Header />
    <Carousel />
    <CarouselModal />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Carousel from './components/Carousel.vue'
import CarouselModal from './components/CarouselModal.vue'

export default {
  name: 'App',
  components: {
    Header,
    Carousel,
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
