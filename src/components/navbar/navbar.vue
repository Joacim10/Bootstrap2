<template>
  <div id="nav">
    <Top></Top>
    <Middle></Middle>
    <Bottom></Bottom>
  </div>
</template>

<script>
import Top from '@/components/navbar/top.vue'
import Middle from '@/components/navbar/middle.vue'
import Bottom from '@/components/navbar/bottom.vue'

export default {
  components: {
    Top,
    Middle,
    Bottom
  }
};
</script>

<style>
</style>