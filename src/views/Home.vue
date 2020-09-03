<template>
  <div class="home">
    <div id="carouselExampleSlidesOnly" class="carousel slide mb-4" data-ride="carousel">
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
    </div>

    <FourCards/>

    <div class="container my-4">
      <div class="text-center">
        <h1 class="d-inline-block">SHOP BY <h1 class="text-info d-inline-block"> CATEGORY </h1></h1>
      </div>
      <div class="text-center">
        <h1 class="d-inline-block">NEW <h1 class="text-info d-inline-block"> ARRIVALS </h1></h1>
      </div>
      <ThreeItems/>
    </div>



      <div class="bg-grey">
        <div class="container">
          <div class="row text-white my-5">
            <div class="col-12 col-sm-6 d-flex justify-content-center justify-content-sm-start">
              <div class="bg-info d-inline-block p-2 py-md-5 text-center d-flex flex-column justify-content-center">
                <h1 class="big-text">30% <span class="small">OFF</span></h1>
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
        </div>
        <ThreeItems/>
      </div>

      <div class="bg-dark">
        <div class="container">
          <div class="row text-white my-5">
            <div class="col-12 col-sm-6 d-flex justify-content-center justify-content-sm-start">
              <div class="bg-info p-4 text-center mb-5 p-0">
                <h1 class="big-text my-0">FLASH</h1>
                <h1 class="big-text my-0">SALE</h1>
                <span class="">UP TO 50% OFF</span>
              </div>
            </div>
            <div class="col-12 col-sm-6 d-flex justify-content-center flex-column my-5">
              <div class="d-flex justify-content-between">
                <div class="d-flex flex-column justify-content-center round bg-white align-items-center">
                  <div class="text-info numbers">7</div>
                  <div class="text-dark">days</div>
                </div>
                <div class="d-flex flex-column justify-content-center round bg-white align-items-center">
                  <div class="text-info numbers">23</div>
                  <div class="text-dark">days</div>
                </div>
                <div class="d-flex flex-column justify-content-center round bg-white align-items-center">
                  <div class="text-info numbers">46</div>
                  <div class="text-dark">days</div>
                </div>
                <div class="d-flex flex-column justify-content-center round bg-white align-items-center">
                  <div class="text-info numbers">12</div>
                  <div class="text-dark">days</div>
                </div>
              </div>
              <div class="text-center">
                <button class="btn btn-light text-info ml-0 rounded">SHOP NOW</button>
              </div>
            </div>
          </div>
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
  .bg-dark {
    background-color: #0E153D;
  }

  .btn-dark {
    background-color: #0E153D;
  }
  .bg-grey {
    background-color: #CCCCCC;
  }
  .rounded {
    margin: 20px;
    border-radius: 50px !important;
  }
  .round {
    border-radius: 50% !important;
    width: 110px;
    height: 110px;
  }
  .big-text {
    font-size: 60px;
    font-family: Play;
    font-weight: bold;
  }
  .numbers {
    font-size: 36px;
    font-family: Play;
    font-weight: bold;
  }
</style>
