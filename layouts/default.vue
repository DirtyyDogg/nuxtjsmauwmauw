<template>
  <section>
    <div id="app" class="appp">
      <div v-if="isMobile">
        Mobiel
        <Mobiel />
      </div>
      <!--  -->
      <div v-else>
        Desktop or Tablet
        <nuxt />
      </div>
    </div>
  </section>
</template>
<script>
import Mobiel from '~/components/Dev/Dev'
export default {
  name: 'App',
  components: {
    Mobiel
  },
  data () {
    return {
      isMobile: true
    }
  }
}
</script>
<style lang="scss" scoped>

</style>
