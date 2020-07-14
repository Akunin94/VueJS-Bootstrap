<template>
   <div id="carouselExampleControls" class="carousel slide carousel-fade" data-ride="carousel" data-interval="4000">
        <ol class="carousel-indicators">
            <li v-for="(slide, index) in slides" :key="slide.index" data-target="#carouselExampleControls" :data-slide-to="index" :class="{ active: index == 0 }"></li>
        </ol>
        <div class="carousel-inner">
            <div v-for="(slide, index) in slides" :key="slide.index" class="carousel-item" :class="{ active: index == 0 }" :data-interval="slide.interval">
                <img class="d-block w-100" :src="slide.icon" :alt="slide.alt" :title="slide.title">
                <div v-if="slide.caption" class="carousel-caption d-none d-lg-block">
                    <h5 v-if="slide.caption.title">First slide label</h5>
                    <p v-if="slide.caption.body">Nulla vitae elit libero, a pharetra augue mollis interdum.</p>
                    <button v-if="slide.caption.button" type="button" class="btn btn-secondary" data-toggle="modal" data-target="#exampleModal">Launch demo modal</button>
                </div>
            </div>
        </div>
        <a class="carousel-control-prev" href="#carouselExampleControls" role="button" data-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="sr-only">Previous</span>
        </a>
        <a class="carousel-control-next" href="#carouselExampleControls" role="button" data-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="sr-only">Next</span>
        </a>
    </div> 
</template>

<script>
export default {
  data() {
      return {
          slides: [
                { 
                    title: 'Pic1', 
                    alt: 'Pic1', 
                    icon: require('@/assets/t1.jpg'),
                    caption: {
                        title: "Заголовок",
                        body : "Тестовый текст",
                        button: true
                    }
                },
                { 
                    title: 'Pic2', 
                    alt: 'Pic2', 
                    icon: require('@/assets/t2.jpg'),
                    caption: {
                        title: "Заголовок1"
                    },
                    interval: 1000
                },
                { 
                    title: 'Pic3', 
                    alt: 'Pic3', 
                    icon: require('@/assets/t3.jpg') 
                }
          ]
      }
  }
}
</script>

<style scoped>
@media all and (min-width: 576px) {
    .carousel-control-next-icon, .carousel-control-prev-icon {
        width: 50px;
        height: 50px;
    }
}
</style>
