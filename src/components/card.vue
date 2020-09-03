<template>
<div>
    <div class="card-main">
            <img :src="require(`@/assets/${item.img}`)" alt="">
        <div class="card-original card-body card-carousel--card--footer">
                <p class="tag" v-for="(tag,index) in item.tag" :key="tag" :class="index &gt; 0 ? 'secondary' : ''">{{ item.tag[index] }}</p>
        </div>
        <div class="card-hover d-none card-body">
            <div class="top-right">
                <i class="my-1 fas fa-circle text-danger"></i>
                <i class="my-1 fas fa-heart"></i>
                <i class="my-1 fas fa-random"></i>
                <i class="my-1 fas fa-search"></i>
                <i class="my-1 fas fa-shopping-cart"></i>
                
            </div>
            <div class="bottom-left">
                <p>{{ item.name }}</p>
                <p class="border d-inline-block p-1 small text-center">fashion</p>
                <div class="">
                    <p class=""><s>${{ item.previous }}</s></p>
                </div>
                <div class="text-info">
                    <h3 class="">${{ item.price }}</h3>
                </div>
            </div>
        </div>
    </div>
</div>

</template>

<script>
export default {
  props: ['item'],

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

    .bottom-left {
        padding: 5px;
        margin: 5px;
        position:absolute;
        bottom: 0px;
        left: 0px;
    }

    p {
        margin-bottom: 2px;
    }


    .card-main {
        position: relative;
        height: 100%;
        overflow: hidden;
        background-color: #EEEEEE;
    }

    .card-main > img {
        object-fit: cover;
        height: 100%;
        object-position: center;
        transform: translateX(-0%);    
}

    .card-body{
        background-color: #0E153D;
        position: absolute;
        z-index: +1;
    }

    .card-original {
        bottom: 0px;
        width: 100%;
    }

    .card-hover {
        opacity: 0.9;
        bottom: 0px;
        height: 100%;
        width: 100%;
    }

    .card-main:hover > .card-original {
        display: none;
    }
    .card-main:hover > .card-hover {
        display: block !important;
    }



</style>