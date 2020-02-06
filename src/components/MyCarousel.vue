<template>
  <div>
      <button>Open gallery</button>
      <button>Previous</button>
      <button>Next</button>
      <button>Close</button>
      <div>
        <img v-bind:key="index" v-for="(url, index) in imgs" :src="url" alt="" width="200"/>
      </div>
  </div>
</template>

<script>
export default {
  name: 'MyCarousel',
  props: {
    imgs: {
        type: Array,
        default: () => []
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
