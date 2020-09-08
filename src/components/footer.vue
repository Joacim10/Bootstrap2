<template>
<div>
        <div class="container my-5">
        <div class="d-flex justify-content-between align-items-center flex-wrap">
          <img src="@/assets/Bexim.png" alt="">
          <img src="@/assets/Lighton.png" alt="">
          <img src="@/assets/Dismis.png" alt="">
          <img src="@/assets/Rosimo.png" alt="">
          <img src="@/assets/Dallas.png" alt="">
        </div>
      </div>

  <div class="background">
    <div class="container">

      <div class="row text-white py-5">
        <div class="col-6 col-sm-4 col-lg-3">
          <Logo class="mb-5" :color="true"/>
          <p class="pb-4">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent enim quam, ullamcorper vel tellus vitae, tempus fringilla lectus. Donec maximus justo eu nisl convallis iaculis. Aenean laoreet.</p>
          <p>Follow us</p>
          <SocialMedia/>
        </div>
        <div class="col-6 col-sm-4 col-lg-3">
          <p class="text-info f-18 font-weight-bold pb-4">CONTACT INFO</p>
          <div class="mb-2">
            <p class="text-info f-16">Address:</p>
            <p class="f-16">Solna Business Park</p>
            <p class="f-16">Feni-2500, Stockholm</p>
          </div>
          <div class="my-2">
            <p class="text-info f-16">Phone:</p>
            <p class="f-16">+08-123456789</p>
            <p class="f-16">+08-123456789</p>
          </div>
          <div class="my-2">
            <p class="text-info f-16">Email:</p>
            <p class="f-16">support@website.com</p>
            <p class="f-16">info@website.com</p>
          </div>
        </div>
        <div class="col-6 d-none d-sm-block col-sm-4 col-lg-3">
          <p class="text-info f-18 pb-4">USEFUL LINKS</p>
          <ul class="pl-0">
            <li><a href="#" class="f-16">Privacy Policy</a></li>
            <li><a href="#" class="f-16">Terms & Conditions</a></li>
            <li><a href="#" class="f-16">Contact Us</a></li>
            <li><a href="#" class="f-16">Our Sitemap</a></li>
            <li><a href="#" class="f-16">Latest News</a></li>
            <li><a href="#" class="f-16">Returns</a></li>
          </ul>
        </div>
        <div class="col-6 d-none d-lg-block col-lg-3">
          <p class="text-info f-18 pb-4">RECENT INSTAGRAM</p>
          <div id="box" class="d-flex flex-column justify-content-between">
            <div class="d-flex justify-content-between h-33">
                <div class="mr-1 w-100 h-100 bg-grey">  </div>
                <div class="mr-1 w-100 h-100 bg-grey">  </div>
                <div class="mr-1 w-100 h-100 bg-grey">  </div>
            </div>
            <div class="d-flex justify-content-between h-33">
                <div class="mr-1 w-100 h-100 bg-grey">  </div>
                <div class="mr-1 w-100 h-100 bg-info text-center d-flex flex-column justify-content-center"> <div><img src="@/assets/instagram.png" alt=""> </div>  </div>
                <div class="mr-1 w-100 h-100 bg-grey">  </div>
            </div>
            <div class="d-flex justify-content-between h-33 ">
                <div class="mr-1 w-100 h-100 bg-grey">  </div>
                <div class="mr-1 w-100 h-100 bg-grey">  </div>
                <div class="mr-1 w-100 h-100 bg-grey">  </div>
            </div>
          </div>

        </div>
      </div>    
    </div>
  </div>
  <div class="bg-black text-white">
    <div class="container">
      <div class="d-flex justify-content-between py-3">
        <div>© Copyright 2020 KenKata</div>
        <div><img src="@/assets/Payment system.png" alt=""></div>
      </div>
    </div>
  </div>



</div>
</template>

<script>
import Logo from '@/components/elements/logo.vue'
import SocialMedia from '@/components/socialmedia/socialmedia.vue'


export default {
    components: {
        Logo,
        SocialMedia
    }
}
</script>

<style scoped>
.background {
  background-color: #0E153D;
}

p {
  margin-bottom: 0.1rem !important;
}

ul > li {
  margin: 0 0 15px 0 ;
}

#box {
  height: 254px;
  width: 255px;
}

.h-100 {
  min-height: 82px;
}

</style>