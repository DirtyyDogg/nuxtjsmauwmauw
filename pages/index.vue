<template>
  <div>
    <ServiceContainer />
    <b-container class="bv-example-row">
    <!--    <b-row align-h="between" cols="4" cols-sm="4" cols-md="4">
        <b-col>
          Column sm 4
        </b-col>
        <b-col>
          Column sm 4
        </b-col>
        <b-col>
          Column sm 4
        </b-col>
        <b-col id="bcolLast">
          Column sm 4
        </b-col>
      </b-row> -->
    </b-container>
  </div>
</template>

<script>
import ServiceContainer from '~/components/Service-Container'
export default {
  components: {
    ServiceContainer
  }
}
</script>

<style lang="scss" scoped>

</style>
