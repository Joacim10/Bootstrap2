<template>
  <div class="home">
    <div id="carouselWithSlides" class="carousel slide mb-4" data-ride="carousel">
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
      <div id="hero" class="">
        <div class="container text-left">
          <h1 class="big-text">Shopping is</h1>
          <h1 class="big-text font-weight-bold text-info">MORE FUN</h1>
          <span id="span-hero">Vivamus dignissim a ex eu ornare. Ut fermentum orci vel diam ultricies faucibus. Quisque quis erat sed</span>
          <div class="">
            <button class="btn btn-light text-info ml-0 rounded">SHOP NOW</button>
          </div>      
        </div>
      </div>
    </div>

    <FourCards class="py-5"/>

    <div class="container my-4">
      <div class="text-center">
        <h1 class="">SHOP BY <h1 class="text-info d-inline-block"> CATEGORY </h1></h1>
        <div class="pb-3">
          <img class="" src="@/assets/curlyrow.png" alt="">
        </div>
        <span>We always try to give you the best product within a fast and reliable way</span>
      </div>

      <Masonry/>


      <div class="text-center pt-5">
        <h1 class="">NEW <h1 class="text-info d-inline-block"> ARRIVALS </h1></h1>
        <div class="pb-3">
          <img class="" src="@/assets/curlyrow.png" alt="">
        </div>
        Check out our latest products from top fashion designers
      </div>

        <div class="container">
          <GeneralCarousel class="d-sm-none" :windowSize="1" :items="items"/>
        </div>
        <GeneralCarousel class="d-none d-sm-block d-md-none" :windowSize="2" :items="items"/>
        <GeneralCarousel class="d-none d-md-block" :windowSize="3" :items="items"/>  

    </div>

    


      <div class="bg-grey">
        <div class="container">
          <div class="row text-white my-5">
            <div class="col-12 col-sm-6 d-flex justify-content-center justify-content-sm-start">
              <div class="bg-info d-inline-block p-2 py-md-5 text-center d-flex flex-column justify-content-center">
                <h1 class="big-text font-weight-bold">30% <span class="small">OFF</span></h1>
                <span>For new customer</span>
                <button class="btn btn-dark d-block rounded">SHOP NOW</button>
              </div>
            </div>
            <div class="col-12 col-sm-6 d-flex justify-content-center flex-column my-3">
              <span class="small pr-5 mr-5">Donec pulvinar arcu vitae ipsum varius cursus. Nunc iaculis fermentum iaculis. Nunc pulvinar purus at erat lacinia, ut convallis nibh consequat. Integer nulla nisi, aliquam at tellus a, viverra scelerisque purus. Nam pretium iaculis ultrices.</span>
              <div>
                <button class="btn btn-light text-info ml-0 rounded">SHOP NOW</button>
              </div>
            </div>
          </div>
        </div>
      </div>


      <div class="container">
        <div class="text-center">
          <h1 class="d-inline-block">FEATURED <h1 class="text-info d-inline-block"> PRODUCTS </h1></h1>
          <div class="pb-3">
            <img class="" src="@/assets/curlyrow.png" alt="">
          </div>
          <span>Check out our monthly featured products from top brands</span>
        </div>
        <GeneralCarousel class="d-sm-none" :windowSize="1" :items="items"/>
        <GeneralCarousel class="d-none d-sm-block d-md-none" :windowSize="2" :items="items"/>
        <GeneralCarousel class="d-none d-md-block" :windowSize="3" :items="items"/>  
      </div>

      <div class="bg-dark">
        <div class="container">
          <div class="row text-white my-lg-5">
            <div class="col-12 col-lg-3 d-flex justify-content-center justify-content-lg-start pb-5">
              <div class="bg-info p-4 text-center mb-lg-5 p-0">
                <h1 class="big-text font-weight-bold my-0">FLASH</h1>
                <h1 class="big-text font-weight-bold my-0">SALE</h1>
                <span class="">UP TO 50% OFF</span>
              </div>
            </div>
            <div class="col-12 col-lg-9 d-flex justify-content-center flex-column my-lg-5">
              <div class="text-center ml-lg-auto">
                <div class="d-flex justify-content-lg-end justify-content-center">
                  <div class="d-flex flex-column justify-content-center round bg-white align-items-center">
                    <div class="text-info numbers">7</div>
                    <div class="text-dark">Days</div>
                  </div>
                  <div class="d-flex ml-3 flex-column justify-content-center round bg-white align-items-center">
                    <div class="text-info numbers">23</div>
                    <div class="text-dark">Hays</div>
                  </div>
                  <div class="d-flex ml-3 flex-column justify-content-center round bg-white align-items-center">
                    <div class="text-info numbers">46</div>
                    <div class="text-dark">Minutes</div>
                  </div>
                  <div class="d-flex ml-3 flex-column justify-content-center round bg-white align-items-center">
                    <div class="text-info numbers">12</div>
                    <div class="text-dark">Seconds</div>
                  </div>
                </div>
                <div class="text-center">
                  <button class="btn btn-light text-info mx-0 rounded">SHOP NOW</button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>

    <div class="container">
      <div class="text-center pt-5">
        <h1 class="">NEW <h1 class="text-info d-inline-block"> ARRIVALS </h1></h1>
        <div class="pb-3">
          <img class="" src="@/assets/curlyrow.png" alt="">
        </div>
        Check out our latest products from top fashion designers
      </div>
      <div class="d-flex justify-content-between">
        <div>
          <Card :item="item1"/>
        </div>
        <div class="d-flex justify-content-between flex-column">
          <div>
            <Card :item="item2"/>
          </div>
          <div>
            <Card :item="item3"/>
          </div>
        </div>
      </div>
    </div>

      <div class="bg-dark my-5">
        <div class="container">
          
          <div id="carouselExampleIndicators" class="carousel slide pb-5" data-interval="false" data-ride="carousel">
            <ol class="carousel-indicators">
              <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>
              <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
              <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
            </ol>
            <div class="carousel-inner">
              <div class="carousel-item active text-center">
                <div class="my-5 text-center">
                  <div>
                    <img src="@/assets/Quote.png" alt="">
                  </div>
                  <div>
                    <img src="@/assets/Testimonial thumb.png" alt="">
                  </div>
                  <div>
                    <img src="@/assets/stars.png" alt="">
                  </div>
                  <h2 class="text-info text-center">Johny Wesmullar</h2>
                    <span class="text-white">CEO, Biotech Inc.</span>
                  <div class="d-flex justify-content-center">
                    <span class="text-white w-50 d-block">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries.</span>
                  </div>
                </div>
              </div>
            </div>
            <a class="carousel-control-prev" href="#carouselExampleIndicators" role="button" data-slide="prev">
              <span class="carousel-control-prev-icon" aria-hidden="true"></span>
              <span class="sr-only">Previous</span>
            </a>
            <a class="carousel-control-next" href="#carouselExampleIndicators" role="button" data-slide="next">
              <span class="carousel-control-next-icon" aria-hidden="true"></span>
              <span class="sr-only">Next</span>
            </a>
          </div>

            <div class="pb-5"></div>
            <div class="pb-5"></div>
        </div>
      </div>

      <div class="container">
        <div class="text-center">
          <h1 class="d-inline-block">LATEST <h1 class="text-info d-inline-block"> BLOG </h1></h1>
          <div class="pb-3">
            <img class="" src="@/assets/curlyrow.png" alt="">
          </div>
          <span>Read our latest posts about our events and trending news</span>
        </div>
        <div class="pb-5">
          <blogCarousel class="d-lg-none" :windowSize="1" :items="items"/>
          <blogCarousel class="d-none d-lg-flex" :windowSize="2" :items="items"/>
        </div>
      </div>

    <Subscribe/>

  </div>
</template>

<script>
import FourCards from '@/components/fourCards.vue'
import GeneralCarousel from '@/components/carousels/generalCarousel.vue'
import Masonry from '@/components/masonry.vue'
import Card from '@/components/card.vue'
import blogCarousel from  '@/components/carousels/blogCarousel.vue'
import Subscribe from  '@/components/elements/subscribe.vue'

export default {
  name: 'Home',
  components: {
    FourCards,
    Masonry,
    Card,
    GeneralCarousel,
    blogCarousel,
    Subscribe
  },
  data: function () {
    return {
    item1: 
        {name: 'Kin Khao', tag: ["Men's denim shirts full"], previous: '220', price: '190', img: 'Product thumb4.png'},
    item2: 
        {name: 'Jū-Ni', tag: ["Women's leather bag and shoe"], previous: '220', price: '190', img: 'Product thumb5.png'},
    item3: 
        {name: 'Delfina', tag: ["New look men's sneakers"], previous: '220', price: '190', img: 'Product thumb6.png'},
    items: [
        {name: 'Kin Khao', tag: ["Winter collection for women's"], previous: '220', price: '190', img: 'Product thumb3.png'},
        {name: 'Jū-Ni', tag: ["Winter collection for women's"], previous: '220', price: '190', img: 'Product thumb.png'},
        {name: 'Delfina', tag: ["Pizza", "Casual"], previous: '220', price: '190', img: 'Product thumb2.png'},
        {name: 'San Tung', tag: ["Chinese", "$$"], previous: '220', price: '190', img: 'Product thumb3.png'},
        {name: 'Anchor Oyster Bar', tag: ["Seafood", "Cioppino"], previous: '220', price: '190', img: 'Product thumb.png'},
        {name: 'Locanda', tag: ["Italian"], previous: '220', price: '190', img: 'Product thumb3.png'},
        {name: 'Garden Creamery', tag: ["Ice cream"], previous: '220', price: '190', img: 'Product thumb.png'},
      ]
    }
  }

}
</script>

<style scoped>

  .btn-dark {
    background-color: #0E153D;
  }
  .bg-grey {
    background-color: #CCCCCC;
  }
  .bg-light-grey {
    background-color: #F6F6F6;
  }
  .rounded {
    margin: 20px;
    border-radius: 50px !important;
  }
  .round {
    border-radius: 50% !important;
    width: 109px;
    height: 109px;
  }
  .big-text {
    font-size: 60px;
    font-family: Play;
  }
  .numbers {
    font-size: 36px;
    font-family: Play;
    font-weight: bold;
    margin-bottom: -12px;
    margin-top: -10px;
  }
  #carouselWithSlides {
    min-height: 453px;
  }

  .carousel-indicators li {
    width: 10px;
    height: 10px;
    border-radius: 100%;
  }

  .carousel-item > img {
    min-height: 453px;
    object-fit: cover;
  }

  #hero {
    position: absolute;
    z-index: +1;
    top: 100px;
    left: 0px;
    width: 100%
  }
  #span-hero{
    width: 35%;
    display: block;
    font-size: 1rem;

  }
</style>
