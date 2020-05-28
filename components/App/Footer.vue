<template>
  <!-- <div id="footer" class="app-footer" style="width: 100%; padding: 32px 0 0 0; position: fixed; bottom: 0; background: linear-gradient(179deg, #353535, #040303); text-align: center; min-height: 47px; max-height: 47px;">
    <div class="container-AppFooter">
      <b-row style="">
        <b-col style="margin:-23px auto auto auto;color: #6d6d6d">
          mauw
        </b-col>
      </b-row>
    </div>
  </div> -->
  <div id="footer" class="fixed-bottomm">
    <h1
      id="test"
    >
      Hooi
    </h1>
  </div>
</template>

<style>
.fixed-bottomm {
    position: absolute;
    right: 0;
    bottom: 0;
    left: 0;
    z-index: 1030;
}
#footer {
    /* background: #3b8070; */
    background: linear-gradient(179deg, #353535, #040303);
    text-align: center;
    height: 36px;
}
h1#test {
    font-size: small;
    margin-top: 11px;
    color: white;
}
</style>
