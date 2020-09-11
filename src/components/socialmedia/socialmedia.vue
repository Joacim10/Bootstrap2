<template>
  <li class="nav-item d-flex align-items-center justify-content-start">
        <a class="nav-link" :class="color" href="#">     
          <i class="fab fa-facebook-f"></i>
        </a>
        <a class="nav-link" :class="color" href="#">     
          <i class="fab fa-twitter"></i>
        </a>
        <a class="nav-link" :class="color" href="#">     
          <i class="fab fa-instagram"></i>
        </a>
        <a class="nav-link" :class="color" href="#">     
          <i class="fab fa-pinterest-p"></i>
        </a>
        <a class="nav-link" :class="color" href="#">     
          <i class="fab fa-youtube"></i>
        </a>
  </li>
</template>

<script>
export default {
  props: ['color'],
/*   data() {
    return {
    color: ''
    }
  } */
}
</script>

<style scoped>
 .nav-link {
   padding: 5px !important;
 }

 a.text-info:focus, a.text-info:hover {
    color: white!important;
}

 a.text-white:focus, a.text-white:hover {
    color: rgba(255, 255, 255, 0.749)!important;
}

</style>