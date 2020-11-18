<template lang="pug">
  div(class="content-grid d-grid")
    Sidebar
    MainContent
</template>

<script>
import Sidebar from '@/components/Sidebar'
import MainContent from '@/components/MainContent'
export default {
  name: 'App',
  components: {
    Sidebar,
    MainContent
  }
}
</script>

<style scoped lang="scss">
.content-grid {
  display: grid;
  grid-template-columns: 20% 70%;
  grid-column-gap: 1fr;
}
</style>
