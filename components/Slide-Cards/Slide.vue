<template>
  <!--  -->
  <b-container class="containerCards">
    <b-row align-v="stretch" align-h="between" cols="1" cols-md="2" cols-lg="4">
      <b-col>
        <Slide1 />
      </b-col>
      <!--  -->
      <b-col>
        <Slide2 />
      </b-col>
      <!--  -->
      <b-col>
        <Slide3 />
      </b-col>
      <!--  -->
      <b-col>
        <Slide4 />
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
import Slide1 from '~/components/Slide-Cards/slide1'
import Slide2 from '~/components/Slide-Cards/slide2'
import Slide3 from '~/components/Slide-Cards/slide3'
import Slide4 from '~/components/Slide-Cards/slide4'
export default {
  components: {
    Slide1, Slide2, Slide3, Slide4
  }
}
</script>

<style lang="scss">
.containerCards.container {
    margin-top: 52px;
}
.containerUP {
  position: relative;
  width: 100%;
  min-height: "20em";
  margin: 0 0 18px 0;
}

.imageUP {
  display: block;
  width: 100%;
  height: auto;
}

.overlayUP {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background-color: #008CBA;
  overflow: hidden;
  width: 100%;
  height: 0;
  transition: .5s ease;
}

.containerUP:hover .overlayUP {
  height: 100%;
}

.textUP {
  color: white;
  font-size: 20px;
  position: absolute;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  text-align: center;
}
// Mobile
@media screen and (min-width: 768px) {
   // UP Styles
   div#cardss {
    display: none
 }
}

// Large
@media screen and (min-width: 992px) {

}

// Larger
@media screen and (min-width: 1200px) {

}

</style>
