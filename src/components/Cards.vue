<template>
   <div class="container-fluid py-5 px-3">
       <h3 class="text-center mb-4">Длинный придлинный заголовок</h3>
       <div class="container">
           <div class="row">
               <div class="col-sm-6 mb-4 col-md-4 col-lg-3 col-xl-3" v-for="card in cards" :key="card.index">
                   <div class="card rounded-0 h-100 shadow-sm">
                       <img v-if="card.image" class="card-img-top rounded-0" :src="card.image" :alt="card.title" :title="card.title">
                       <div class="card-body p-3" v-if="card.title || card.text || card.link">
                           <h5 v-if="card.title">{{ card.title }}</h5>
                           <h6 v-if="card.subtitle" class="text-muted mb-3">{{ card.subtitle }}</h6>
                           <p v-if="card.text" class="card-text">{{ card.text }}</p>
                       </div>
                        <ul v-if="card.list" class="list-group list-group-flush">
                            <li class="list-group-item" v-for="list in card.list" :key="list.index">
                                {{ list }}
                            </li>
                        </ul>
                        <div v-if="card.link" class="card-body d-flex align-items-end">
                            <a :href="card.link" class="btn btn-secondary rounded-0">Подробнее</a>
                        </div>
                   </div>
               </div>
           </div>
       </div>
   </div>
</template>

<script>
export default {
  data() {
      return {
          cards: [
              {
                  title: "Title1",
                  subtitle: "Subtitle1 1 1 1 1 1 1 1 1",
                  text: "Text1",
                  link: "/test1",
                  image: require('@/assets/t1.jpg') 
              },
              {
                  title: "Title2",
                  subtitle: "Subtitle2",
                  text: "Text2",
                  link: "/test2",
                  image: require('@/assets/t2.jpg') 
              },
              {
                  title: "Title3",
                  subtitle: "Subtitle3",
                  text: "Text3",
                  link: "/test3",
                  image: require('@/assets/t3.jpg') 
              },
              {
                  title: "Title4",
                  subtitle: "Subtitle4",
                  text: "Text4",
                  link: "/test4",
                  image: require('@/assets/t2.jpg') 
              },
              
              {
                  title: "Title1",
                  subtitle: "Subtitle1 1 1 1 1 1 1 1 1",
                  text: "Text1",
                  link: "/test1",
                  image: require('@/assets/t1.jpg'),
                  list: [
                      'Cras justo odio',
                      'Dapibus ac facilisis in',
                      'Vestibulum at eros'
                  ]
              },
              {
                  title: "Title2",
                  subtitle: "Subtitle2",
                  text: "Text2",
                  link: "/test2",
                  image: require('@/assets/t2.jpg') 
              },
              {
                  title: "Title3",
                  subtitle: "Subtitle3",
                  text: "Text3",
                  link: "/test3",
                  image: require('@/assets/t3.jpg') 
              },
              {
                  title: "Title4",
                  subtitle: "Subtitle4",
                  text: "Text4",
                  link: "/test4",
                  image: require('@/assets/t2.jpg') 
              }
          ]
      }
  }
}
</script>

<style>
</style>
