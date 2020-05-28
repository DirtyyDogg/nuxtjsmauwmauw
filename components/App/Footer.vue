<template>
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
    bottom: -1px;
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
