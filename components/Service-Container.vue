<template>
  <section class="containerServicer">
    <Carousel />
    <Slide />
  </section>
</template>

<script>
import Slide from '~/components/Slide-Cards/Slide'
import Carousel from '~/components/Carousel/Carousel'

export default {
  components: {
    Slide, Carousel
  }
}
</script>

<style lang="scss">
.img-fluid {
    height: 81vh !important;
}
// Larger
@media screen and (min-width: 800px) {
    .img-fluid {
        height: 70vh !important;
    }
}
@media screen and (min-width: 1000px) {
    .img-fluid {
        height: 70vh !important;
    }
}
</style>
