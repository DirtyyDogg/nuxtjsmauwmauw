<template>
  <b-container id="intro" style="text-align: center;">
    <div>
      <logo />
      <h1 class="title">
        {{ SiteTitle }}
      </h1>
      <h2 class="subtitle">
        My astonishing Nuxt.js project
      </h2>
      <div class="links">
        <a
          href="https://nuxtjs.org/"
          target="_blank"
          class="button--green"
        >
          Documentation
        </a>
        <a
          href="https://github.com/nuxt/nuxt.js"
          target="_blank"
          class="button--grey"
        >
          GitHub
        </a>
      </div>
    </div>
  </b-container>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  },
  data () {
    return {
      SiteTitle: 'MauwMauw'
    }
  }
}
</script>

<style>
@media only screen and (max-width: 576px) {
  /* .wrapper {
    background-color: lightblue;
  } */
  .title {
      font-size: 79px;
  }
}
</style>
