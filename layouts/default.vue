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

</style>
