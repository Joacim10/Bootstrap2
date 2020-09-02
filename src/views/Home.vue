<template>
  <div class="home">
    <div id="carouselExampleSlidesOnly" class="carousel slide" data-ride="carousel">
      <div class="carousel-inner">
        <div class="carousel-item active">
          <img class="d-block w-100" src="../assets/Background-1.png" alt="First slide">
        </div>
        <div class="carousel-item">
          <img class="d-block w-100" src="../assets/Background-1.png" alt="Second slide">
        </div>
        <div class="carousel-item">
          <img class="d-block w-100" src="../assets/Background-1.png" alt="Third slide">
        </div>
      </div>
      <FourCards/>
      <div class="container">
        <ThreeItems/>
      </div>
    </div>
  </div>
</template>

<script>
import FourCards from '@/components/fourcards.vue'
import ThreeItems from '@/components/carousels/threeitems.vue'

export default {
  name: 'Home',
  components: {
    FourCards,
    ThreeItems
  }
}
</script>

<style scoped>
  .home {
    height: 4000px;
  }
</style>
