<template>
  <!--  -->
  <b-container class="containerCards">
    <div class="test">
      ok
    </div>
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
    <div class="fill">
      <h1 />
    </div>
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
/* Voor PC */
@media screen and (min-width: 992px) {
  .test {
    display: none;
  }
  .containerCards.container {
      background: #80008000;
      padding: 25px 7px 0px 7px;
      margin-top: 0px;
  }
}
@media screen and (max-width: 600px) {
  .test {
    background-color: #ff000000;
    min-height: 3px;
    max-height: 7px;
  }
  .containerCards.container {
      background: #80008000;
      padding: 25px 7px 0px 7px;
      margin-top: 0;
  }
}

// @media only screen and (min-width: 500px) {
//   /* For tablets: */
//   .test {
//       background: #ff000000;
//       min-height: 3px;
//       max-height: 7px;
//   }
//   .containerCards.container {
//       background: #1f1f1fc2;
//       padding: 25px 7px 0px 7px;
//       margin-top: 0;
//   }
// }
.fill {
    padding: 8vh;
}
// .containerCards.container {
//     margin-top: 20px;
// }
.containerCards.container .row {
    margin-top: -16px;
    margin-bottom: -90px;
}
.containerCards.container {
    // margin-top: 54px;
    // margin-top: 16px;
    // background: rgba(0, 255, 255, 0.0);
    // padding: 7px 7px 7px 7px;
    // padding: 15px 7px 0px 7px;
    position: relative;
    margin-left: auto;
    margin-right: auto;
    // top: 50%;
    height: 100%;
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
#card1.containerUP > .overlayUP {
    background-color: rgba(152, 218, 47, 0.88);
    // background-color: #98da2fbd;
}
#card1.containerUP > .overlayUP > .textUP {
    color: white;
    text-shadow: 2px 2px 4px #000000;
    // text-shadow: 0 1px 0 #ccc,
    //            0 2px 0 #c9c9c9,
    //            0 3px 0 #bbb,
    //            0 4px 0 #b9b9b9,
    //            0 5px 0 #aaa,
    //            0 6px 1px rgba(0,0,0,.1),
    //            0 0 5px rgba(0,0,0,.1),
    //            0 1px 3px rgba(0,0,0,.3),
    //            0 3px 5px rgba(0,0,0,.2),
    //            0 5px 10px rgba(0,0,0,.25),
    //            0 10px 10px rgba(0,0,0,.2),
    //            0 20px 20px rgba(0,0,0,.15);
}
#card2.containerUP > .overlayUP {
    background-color: #de57c7b3;
}
#card3.containerUP > .overlayUP {
    background-color: #57acdea6;
}
#card4.containerUP > .overlayUP {
    background: #0a0a0ea6;
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
  text-shadow: 2px 2px 4px #000000;
  font-size: 20px;
  position: absolute;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  text-align: center;
}
// // Mobile
// @media screen and (min-width: 768px) {
//    // UP Styles
//    div#cardss {
//     display: none
//  }
 // .container-xl {
   //  margin-top: 14px;
// }
// .img-fluid {
    // 70vh !important;
 // }
//}

// Large
@media screen and (min-width: 1200px) {
    .container-xl {
        max-width: unset;
    }
}

.Slider.container-xl {
    margin-top: 8px;
    // margin-left: auto;
    // margin-right: auto;
    padding: 0 5px 0 5px;
    // padding: 0 8px 0 8px;
}
.img-fluid {
    height: 80vh !important;
}
</style>
