<template>
  <!--  -->
  <div class="containerIO">
    <img src="https://www.w3schools.com/howto/img_avatar.png" class="imageIO">
    <div class="overlayIO">
      <a href="#" class="iconIO" title="User Profile">
        <i class="fas fa-user" />
      </a>
      <div class="textIO">
        Hello World
      </div>
    </div>
  </div>
</template>

<script>

</script>

<style lang="scss" scoped>
// IO Styles
.containerIO {
  position: relative;
  width: 100%;
  max-width: 400px;
}

.imageIO {
  display: block;
  width: 100%;
  height: auto;
}
.overlayIO {
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  width: 100%;
  opacity: 0;
  transition: .3s ease;
  background-color: red;
}
.containerIO:hover .overlayIO {
  opacity: 1;
}
.iconIO {
  color: white;
  font-size: 100px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  text-align: center;
}
.textIO {
  color: white;
  font-size: 20px;
  position: absolute;
  top: 50%;
  bottom: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  text-align: center;
}
</style>
