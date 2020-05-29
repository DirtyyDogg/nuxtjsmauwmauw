<template>
  <section class="containerHome">
    <Carousel />
    <Slide />
    <ServicesBox />
  </section>
</template>

<script>
import Slide from '~/components/Slide-Cards/Slide'
import Carousel from '~/components/Carousel/Carousel'
import ServicesBox from '~/components/ServicesBox/Services'

export default {
  components: {
    Slide, Carousel, ServicesBox
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
    background-color: #ffc3c3;
    border-top: 1px solid rgba(115, 115, 115, 0.65);
    border-bottom: 1px solid rgb(21, 1, 7);
    border-left: 1px solid rgba(0, 0, 0, 0.9);
    border-right: 1px solid rgba(114, 125, 69, 0.9);
    border-radius: 6px;
    opacity: 0.9;
    width: 34px;
    height: 5px;
    box-shadow: #000 43px 61px 32px;
}
.img-fluid {
    // height: 86vh !important;
    max-height: 100vh !important;
}
.slurp {
    // margin: 94px;
    // padding: 66px;
    margin: 0px;
    background: #ff000000;
    display: none;
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
        bottom: 64px;
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
