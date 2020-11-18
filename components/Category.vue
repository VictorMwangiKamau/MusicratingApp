<template lang="pug">
  div(class="mb-5" v-on:load="showAngles")
    h3(class="subtitle") Category
    VueSlickCarousel(:arrows="true" :dots="true")
      div(class="d-grid columns-3")
        nuxt-link(to="/") 
          div(class="card")
            div(class="card-body")
              div(class="card-header")
                p(class="lead") Gengetone

        nuxt-link(to="/") 
          div(class="card")
            div(class="card-body")
              div(class="card-header")
                p(class="lead") Gengetone

        nuxt-link(to="/") 
          div(class="card")
            div(class="card-body")
              div(class="card-header")
                p(class="lead") Gengetone

      div(class="d-grid columns-3")
        nuxt-link(to="/") 
          div(class="card")
            div(class="card-body")
              div(class="card-header")
                p(class="lead") Gengetone

        nuxt-link(to="/") 
          div(class="card")
            div(class="card-body")
              div(class="card-header")
                p(class="lead") Gengetone

        nuxt-link(to="/") 
          div(class="card")
            div(class="card-body")
              div(class="card-header")
                p(class="lead") Gengetone

      div(class="d-grid columns-3")
        nuxt-link(to="/") 
          div(class="card")
            div(class="card-body")
              div(class="card-header")
                p(class="lead") Gengetone

        nuxt-link(to="/") 
          div(class="card")
            div(class="card-body")
              div(class="card-header")
                p(class="lead") Gengetone

            div


</template>

<script>
import VueSlickCarousel from 'vue-slick-carousel'
import 'vue-slick-carousel/dist/vue-slick-carousel.css'
// optional style for arrows & dots
import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'

export default {
  name: 'Category',
  components: {
    VueSlickCarousel
  },
  methods: {
    showAngles() { 
      document.querySelector('.slick-prev').innerHTML `<i class="fas fa-angle-left"></i>`
      document.querySelector('.slick-next').innerHTML `<i class="fas fa-angle-right"></i>`
      document.querySelector('.slick-prev').style.color = 'black'
      document.querySelector('.slick-prev').style.color = 'black'

    }
  }
}
</script>

<style scoped lang="scss">
.card {
  background-color: var(--pendeza-danger);
  height: 5rem;
  color: var(--pendeza-light);
  text-align: center;
  padding-top: 6%;

}


.slick-prev, .slick-next {
  color: black;
}
button {
  background-color: black;
}
</style>
