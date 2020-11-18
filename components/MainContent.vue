<template lang="pug">
  main(class="main px-3 pt-1")
    Category
    SongList
</template>

<script>
import Category from '@/components/Category'
import SongList from '@/components/SongList'
export default {
  name: 'MainContent',
  components: {
    Category,
    SongList
  }
}
</script>

<style scoped lang="scss">
</style>
