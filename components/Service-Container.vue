<template>
  <b-container class="containerService">
    <b-row align-v="stretch" align-h="between" cols="4" cols-sm="4" cols-md="4">
      <b-col>
        <div class="containerSlide">
          <img src="https://www.w3schools.com/howto/img_avatar.png" alt="Avatar" class="image">
          <div class="overlayy">
            <a href="#" class="icon" title="User Profile">
              <i class="fas fa-user" />
            </a>
          </div>
        </div>
      </b-col>
      <b-col>
        <p>Column sm 4</p>
        <p>Column sm 4</p>
        <p>Column sm 4</p>
        <!-- <img src="https://www.w3schools.com/howto/img_avatar.png" alt="Avatar" class="image"> -->
      </b-col>
      <b-col>
        <p>Column sm 4</p>
        <p>Column sm 4</p>
        <p>Column sm 4</p>
        <!-- <img src="https://www.w3schools.com/howto/img_avatar.png" alt="Avatar" class="image"> -->
      </b-col>
      <b-col id="bcolLast">
        <p>Column sm 4</p>
        <p>Column sm 4</p>
        <p>Column sm 4</p>
        <!--  -->
      </b-col>
    </b-row>
  </b-container>
</template>

<style lang="scss" scoped>
@media screen and (min-width: 992px) {
    div#bcolLast {
    margin: 0 -83px 0 0;
    }
}
.containerSlide {
  position: relative;
  width: 100%;
  max-width: 400px;
}

.image {
  display: block;
  width: 100%;
  height: auto;
}
.overlayy {
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
.containerSlide:hover .overlayy {
  opacity: 1;
}
.icon {
  color: white;
  font-size: 100px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  text-align: center;
}

</style>

<script>
export default {
  components: {
    //
  }
}
</script>
