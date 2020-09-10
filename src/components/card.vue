<template>
<div>
    <div class="card-main">
        <img :src="require(`@/assets/${item.img}`)" alt="">
        <div class="top-left">
            <div class="circle text-white p-1 text-center d-none" :class="item.badge" >{{item.badge}}</div>
            <div class="circle text-white p-1 text-center d-none" :class="item.discount" >{{item.discountAmount}}</div>
        </div>

        <div class="card-original card-body card-carousel--card--footer">
            <p class="f-18" >{{ item.name }}</p>
        </div>
        <div class="card-hover card-body p-1 p-sm-2">
            <div class="top-right">
                <i class="my-1 fas fa-circle text-danger"></i>
                <i class="my-1 fas fa-heart"></i>
                <i class="my-1 fas fa-random"></i>
                <i class="my-1 fas fa-search"></i>
                <i class="my-1 fas fa-shopping-cart"></i>
            </div>
            <div class="bottom-left text-white">
                <p class="f-18">{{ item.name }}</p>
                <p class="border d-inline-block p-1 small text-center">{{ item.tag }}</p>
                <div class="">
                    <p class=""><s>${{ item.previous }}</s></p>
                </div>
                <div class="text-info">
                    <h3 class="">${{ item.price }}</h3>
                </div>
            </div>
            <div class="bottom-right text-info d-none" :class="{ 'd-block' : item.stars >= 0}">
                <i v-for="(stars, index) in item.stars" :key="index" class="fas fa-star"></i>
                <i v-for="item in nonFilledStars" :key="'nonFilled'+item" class="far fa-star"></i>
            </div>
        </div>
    </div>
</div>

</template>

<script>
export default {
  props: ['item'],
  data() {
      return {
          nonFilledStars: Number
      }
  },
  mounted: function() {
      this.nonFilledStars = 5 - (this.item.stars || 0)
  }
}
</script>

<style scoped>

    .top-right {
        position:absolute;
        right: 0px;
        top: 0px;
        display: flex;
        flex-direction: column;
        justify-content: between;
        align-items: center;
        background-color: white;
        border-radius: 20px;
        padding: 5px;
        margin: 5px;
    }

    .top-left {
        position:absolute;
        left: 0px;
        top: 0px;  
        padding: 20px 20px 0;
    }

    .circle {
        border-radius: 50%;
        padding: 5px;
        margin-bottom: 10px;
        width: 60px;
        height: 60px;
        display: flex;
        justify-content: center;
        align-content: center;
        flex-direction: column;
    }

    .card-main:hover .top-left {
        display: none !important;
    }

    .bottom-left {
        padding: 5px;
        margin: 5px;
        position:absolute;
        bottom: 0px;
        left: 0px;
    }

    .bottom-right {
        padding: 5px;
        margin: 5px;
        position:absolute;
        bottom: 0px;
        right: 0px;
    }

    p {
        margin-bottom: 2px;
    }

    .card-main {
        position: relative;
        height: 100%;
        width: 100%;
        overflow: hidden;
        background-color: #EEEEEE;
    }

    .card-main > img {
        object-fit: cover;
        height: 100%;
        width: 100%;
        object-position: center;
        transform: translateX(-0%);    
}

    .card-body{
        background-color: #0E153D;
        position: absolute;
        z-index: +1;
        padding: 10px;
    }

    .card-original {
        bottom: 0px;
        width: 100%;
    }

    .card-hover {
        transition: bottom 0.3s ease;
        bottom: -100%;
        opacity: 0.9;
        height: 100%;
        width: 100%;
    }

    .card-main:hover > .card-original {
        display: none;
    }
    .card-main:hover > .card-hover {
        bottom: 0;
        display: block !important;
    }

    .NEW {
        background-color: #20D3C2;
        display: flex !important;
    }

    .HOT {
        background-color: red;  
        display: flex !important;
    }

    .discount {
        background-color: #64CB83; 
        display: flex !important;
    }

</style>