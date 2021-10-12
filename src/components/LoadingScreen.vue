<template>
  <div class="" v-if="status">
    I AM LOADING, Status: {{status}}
  </div>
</template>

<script>
export default {
  name: 'LoadingScreen',
  props: {
    status: Boolean
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
