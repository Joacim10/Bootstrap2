<template>
<div>
    <div class="card-main">
        <div class="left">
        </div>
        <div class="right">
            <div class="text-white ml-3 pb-2 px-1 mb-2 pb-2">
                <div class="d-inline-block py-2 px-1 mb-2 bg-info">
                    <div class="text-center">
                        <div class="font-weight-bold">
                            24 {{item.date}}
                        </div> 
                        JULY
                    </div>
                </div>
                <p class="f-14">By {{item.author}}</p>
                <p class="f-16 text-info pr-1">{{item.titel}}</p>
                <div>
                    <p class="mr-2 mt-2 border f-14 d-inline-block p-1 small text-center">Travel</p>
                    <p class="border f-14 d-inline-block p-1 small text-center">Fashion</p>
                </div>
                <button class="ml-0 my-3 f-16 btn btn-white text-info rounded">Read more</button>
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

    .left {
        position: absolute;
        width: 65%;
        height: 100%;
        z-index: +1;
        left: 0;
        top: 0;
        background-color: #CCCCCC;
    }

    .right {
        position: absolute;
        z-index: +2;
        min-height: 75%;
        width: 50%;
        right: 0;
        top: 12.5%;
        background-color: #0E153D;
    }

    p {
        margin-bottom: 2px;
    }


    .card-main {
        position: relative;
        height: 350px;
        width: 100%;
        overflow: hidden;
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

</style>