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
    html, body {
        height: 100%;
        width: 100%;
        background: #fff0;
    }
    .app {
        overflow:hidden
    }
    ::-webkit-scrollbar {
        width: 0px !important;
    }
    .wrapper {
        margin: auto;
        margin-bottom: -50px;
        padding: 0 0 115px 0;
        /* max-height: 98.3vh; */
        max-height: 100vh;
        min-height: 100vh;
        background: black;
        overflow: scroll;
    }
    .navbar-collapse.show {
        max-height: 100vh;
        min-height: 100vh;
        text-align: center;
    }

    @media screen and (max-width: 600px) {
    /* mobile */
    /* */
    /* div#intro {
        background: #1f1e1ed1;
    }
    div#intro.container {
        text-align: center;
        margin: -29px 0 0 0;
        background: yellowgreen;
    } */
    .wrapper {
        margin: auto;
        margin-bottom: -50px;
        padding: 0 0 115px 0;
        /* max-height: 98.3vh; */
        max-height: 100vh;
        min-height: 100vh;
        background: black;
        overflow: scroll;
    }
}
</style>
