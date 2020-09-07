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

.f-14 {
  font-size: 0,875rem;
}
.f-16 {
  font-size: 1rem;
}
.f-18 {
  font-size: 1.125rem;
}
.f-24 {
  font-size: 1.5rem;
}
.f-36 {
  font-size: 2.25rem;
}
.f-play {
  font-family: play;
}

body {
  font-family: roboto;
}

a {
  color: white;
}

ul {
  list-style-type: none;
}

.bg-black {
  background-color: #080C24;
}

.bg-dark {
  background-color: #0E153D !important;
}

.bg-info {
  background: #20D3C2 !important;
}

.bg-grey {
  background-color: #CCCCCC;
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
