<template lang="pug">
  div(class="navbar mb-0 dark darken-1")
    div(class="navbar-body wrapper-responsive")
      span(class="navbar-brand text-extralarge") ktunes
      div(class="search-bar")
        input(class="navbar-input" placeholder="song..." style="border-color: var(--pendeza-danger); width: 60%; border-radius: none" type="search")
        i(class="fas fa-search text-large danger py-1 px-1")
      span(class="danger navbar-button h-4") Account
</template>

<script>
export default {
  name: 'Navbar'
}
</script>

<style scoped lang="scss">
.search-bar {
  display: flex;
  justify-content: flex-start;
  
}
</style>
