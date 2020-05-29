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
.form-inline {
    display: flex;
    flex-flow: column;
    align-items: center;
    padding: 0px 0 0 0;
}
.form-inline > button {
    padding: 0 3px 0 3px;
    margin: 0;
    position: relative;
    top: 9px;
}
.carousel-option {
    bottom: 0;
    top: 37%;
}
.carousel-caption {
    bottom: 134px;
}
.carousel-indicators {
    bottom: 0;
}
.carousel-indicators li {
    background-color: #fff;
    border-top: 0.1px solid rgba(0, 0, 0, 0.87);
    border-bottom: 0.1px solid rgba(10, 10, 39, 0.9);
    border-left: 0.1px solid rgba(0, 0, 0, 0.9);
    border-right: 0.1px solid rgba(45, 45, 45, 0.9);
    border-radius: 6px;
    opacity: 0.9;
    width: 34px;
    height: 7px;
}
.img-fluid {
    // height: 86vh !important;
    height: 106vh !important;
    max-height: 100vh !important;
}
.slurp {
    // margin: 94px;
    // padding: 66px;
    margin: 0px;
    background: #ff000000;
    display: block;
    // position: static;
    position: relative;
    padding: 0px 0 0 0;
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
    .carousel-indicators {
        bottom: 33px;
    }
    .form-inline {
        display: flex;
        flex-flow: wrap;
        align-items: center;
        padding: 0px 0 0 0;
}
    .form-inline > button {
        padding: 0 4px 0 4px;
        margin: 0;
        position: relative;
        top: 0;
}
}
</style>
