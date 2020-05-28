<template>
  <!--  -->
  <div class="containerUP">
    <img src="https://www.w3schools.com/howto/img_avatar.png" class="imageUP">
    <div class="overlayUP">
      <div class="textUP">
        Hello World
      </div>
    </div>
  </div>
</template>

<script>

</script>

<style lang="scss">
// UP Styles
.containerUP {
  position: relative;
  width: 100%;
  min-height: 7cm;
}

.imageUP {
  display: block;
  width: 100%;
  height: auto;
}

.overlayUP {
  position: absolute;
  bottom: 0px;
  left: 0;
  right: 0;
  background-color: #008CBA;
  overflow: hidden;
  width: 100%;
  height: 0;
//   height: 63px;
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
@media screen and (max-width: 500px) {
   // UP Styles
}

// Large
@media screen and (min-width: 992px) {
    //     // UP Styles
    .overlayUP {
        bottom: 53px;
    }
    .containerUP {
        height: 36%;
    }
}

// Larger
@media screen and (min-width: 1200px) {
    // UP Styles
    .overlayUP {
        bottom: 12px;
    }
}

// /
//     .containerUP {
//         position: relative;
//         width: 100%;
//         min-height: 7cm;
//     }
//     .overlayUP {
//         position: absolute;
//         bottom: 10px;
//         left: 0;
//         right: 0;
//         background-color: #008CBA;
//         overflow: hidden;
//         width: 100%;
//         height: 0;
//         //   height: 63px;
//         transition: .5s ease;
//     }

//     .containerUP:hover .overlayUP {
//         height: 100%;
//     }
// }
// /
// // Mobile

</style>
