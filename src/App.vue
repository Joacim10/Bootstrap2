<template>
  <div id="app">
    <Navbar class="sticky-top bg-white"/>  
    <router-view/>
    <Footer/>
  </div>

</template>

<script>
import Navbar from '@/components/navbar/navbar.vue'
import Footer from '@/components/footer.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Footer
  }
}
</script>

<style>
body {
  font-family: roboto;
}

a {
  color: white;
}

ul {
  list-style-type: none;
}

.bg-info {
  background: #20D3C2 !important;
}

.text-info {
  color: #20D3C2 !important;
}

.btn-info {
  background: #20D3C2 !important;
}

.badge-info {
  background: #20D3C2 !important;
}

</style>
