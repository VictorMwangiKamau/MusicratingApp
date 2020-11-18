<template lang="pug">
  div(class="dark pt-1 text-light")
    ul(class="list")
      nuxt-link(to="/")
        li(class="list-item") 
          i(class="fas fa-home")
            small(class="ml-1") Home
      li(class="list-item") 
        i(class="fas fa-download")
          small(class="ml-1") Download
      nuxt-link(to="/category")
        li(class="list-item") 
          i(class="fas fa-ome")
            small(class="ml-1") Category
      nuxt-link(to="/artists")
        li(class="list-item") 
          i(class="fas fa-person")
            small(class="ml-1") Artists
      nuxt-link(to="/latest")
        li(class="list-item") 
          i(class="fas fa-person")
            small(class="ml-1") Latest
</template>

<script>
export default {
  name: 'Sidebar'
}
</script>

<style scoped lang="scss">
ul {
  li {
    cursor: pointer;
  }
  li:hover {
      color: var(--pendeza-danger);
      transition: color ease-in 0.3s;
  }
}
</style>
