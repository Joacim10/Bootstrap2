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

.fa-chevron-down {
    margin-left: 8px;
    color: #20D3C2;
    font-size: 13px;
}

.outline-grey{
  border: 1px solid #E3E3E3;
}
</style>