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
    height: 79vh !important;
}
.slurp {
    margin: 49px;
    // padding: 66px;
    background: #ff000000;
    display: block;
    position: static;
}
// Larger
@media screen and (min-width: 800px) {
    .img-fluid {
        height: 70vh !important;
    }
}
@media screen and (min-width: 1000px) {
    .img-fluid {
        height: 67vh !important;
    }
    .Slider.container-xl {
        margin-top: 13px;
    }
    .slurp {
        display: none;
    }
}
</style>
