<template>
  <header class="h-100vh scroll-none">
    <video src="./../assets/images/video.mp4" autoplay muted loop class="video-responsive absolute left-0 right-0 top-0"></video>
    <div class="wrapper text-center z-index-top">
      <h3>Sorry, the page was not found</h3>
      <nuxt-link to="/">
        <button class="dark large">Home</button>
      </nuxt-link>
    </div>
  </header>
</template>

<script>
export default {};
</script>

<style scoped lang="scss" scoped>
.text-extralarge {
  font-size: 6rem;
}

header {
  position: relative;

  div {
    padding-top: 10%;
    min-height: 100vh;
  }
}
</style>
