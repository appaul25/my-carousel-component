<template>
  <div id="app">
    <MyCarousel :imgs="carouselImagesUrls"/>
  </div>
</template>

<script>
import MyCarousel from './components/MyCarousel.vue'

export default {
  name: 'app',
  components: {
    MyCarousel
  },
  data() {
    return {
      carouselImagesUrls: [
        'assets/img/photo-1.jpg',
        'assets/img/photo-2.jpg',
        'assets/img/photo-3.jpg',
        'assets/img/photo-4.jpg',
        'assets/img/photo-5.jpg',
      ]
    }
  },
}
</script>

<style>
body {
  margin: 0;
}
</style>
