<template>
<div>
    <div class="card-main">
        <div class="left">
        </div>
        <div class="right">
            <div class="bg-info d-inline-block text-white ml-3 py-2 px-1 mb-2">
                <div class="text-center">
                    <div class="font-weight-bold">
                        24 {{item.date}}
                    </div> 
                    JULY
                </div>
            </div>
            <p class="tag" v-for="(tag,index) in item.tag" :key="tag" :class="index &gt; 0 ? 'secondary' : ''">{{ item.tag[index] }}</p>
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
        width: 50%;
        height: 70%;
        z-index: +2;
        right: 0;
        top: 15%;
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