<template>
  <div>
    <div class="container">
        Products
    </div>
    <FourCards/> 
    <Subscribe/> 
  </div>
</template>

<script>
import FourCards from '@/components/fourCards.vue'
import Subscribe from  '@/components/elements/subscribe.vue'

export default {
  name: 'Products',
  components: {
    FourCards,
    Subscribe
  }
}
</script>

<style>

</style>