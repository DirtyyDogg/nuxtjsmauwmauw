<template>
  <div class="app">
    <appHeader />
    <div class="wrapper">
      <nuxt />
    </div>
    <appFooter />
  </div>
</template>

<script>
import appHeader from '~/components/App/Header'
import appFooter from '~/components/App/Footer'
export default {
  components: {
    appHeader, appFooter
  }
}
</script>

<style>
    html {
        overflow: hidden;
    }
    body {
        background-color: #1d1d1d;
    }
    .app {
        overflow:hidden
    }
    ::-webkit-scrollbar {
        width: 0px !important;
    }
    .wrapper {
        margin: auto;
        padding: 25px 0px 60px 0;
        max-height: 85vh;
        background: black;
        overflow: scroll;
    }
    .navbar-collapse.show {
        max-height: 367px;
        min-height: 535px;
    }
</style>
