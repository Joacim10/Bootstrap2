<template>
  <div class="container">
    <div class="grid-container">
      <div class="menu text-left">
        <div class="f-16 text-info">Product Categories</div>
      </div>
      <div class="products">Main</div>  
      <div class="pagination">Pagination</div>
    </div>
    <Subscribe/> 
  </div>
</template>

<script>
import Subscribe from  '@/components/elements/subscribe.vue'

export default {
  components: {
    Subscribe
  }
}
</script>

<style scoped>
.menu { grid-area: menu; }
.products { grid-area: products; }
.pagination { grid-area: pagination; }

.grid-container {
  display: grid;
  grid-template-areas:
    'menu products products products products'
    'menu products products products products'
    'menu products products products products'
    'menu products products products products'
    'menu pagination pagination pagination pagination';
  grid-gap: 10px;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
}
</style>