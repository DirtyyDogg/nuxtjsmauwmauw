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
    .wrapper {
        margin: auto;
        padding: 25px 0px 60px 0;
        max-height: 85vh;
        overflow: auto scroll;
        overflow-x: hidden;
        overflow-y: scroll;
        background: black;
    }
    .navbar-collapse.show {
        max-height: 367px;
        min-height: 535px;
    }
</style>
