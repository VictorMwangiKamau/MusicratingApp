<template lang="pug">
  main(class="main")
    h3(class="subtitle") Songs 
    div(class="list-song-grid d-grid columns-2-on-phone columns-3-on-tablet columns-4-on-laptop grid-column-gap-1")
      div(class="song-list d-grid" v-for="song in songs")
        div(class=" card song-card")
          div(class="card-body")
            div(class="card-header")
              img(class="image-responsive" src="./../assets/images/background-image-2.jpg")
            div(class="card-footer d-flex justify-between")
              span(class="card-text") {{ song.text }}
              span
                i(class="fas fa-thumbs-up text-danger mr-2 cursor-pointer")
                i(class="fas fa-thumbs-down cursor-pointer")
</template>

<script>
export default {
  name: 'SongList',
  components: {
  },
  data() {
    return {
      songs: [
        {
          name: 'some song',
          text: 'some text',
          url: './../assets/images/background-image-2.jpg'
        },
        {
          name: 'some song',
          text: 'some text',
          url: './../assets/images/background-image-2.jpg'
        },{
          name: 'some song',
          text: 'some text',
          url: './../assets/images/background-image-2.jpg'
        },{
          name: 'some song',
          text: 'some text',
          url: './../assets/images/background-image-2.jpg'
        },{
          name: 'some song',
          text: 'some text',
          url: './../assets/images/background-image-2.jpg'
        },{
          name: 'some song',
          text: 'some text',
          url: './../assets/images/background-image-2.jpg'
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
.list-song-grid {
  .card {
    .card-body {
      padding-left: 0;
      padding-right: 0;
      
      .card-header {
        img {
          box-shadow: none;
        }
      }

      .card-footer {;
        padding-right: 0.5rem;
        padding-left: 0.5rem;
      }
    }
  }
}
</style>
