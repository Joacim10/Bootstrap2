<template>
    <div class="card-main">
            <img src="https://placehold.it/200x200"/>
        <div class="card-original card-body card-carousel--card--footer">
                <p>{{ item.name }}</p>
                <p class="tag" v-for="(tag,index) in item.tag" :key="tag" :class="index &gt; 0 ? 'secondary' : ''">{{ item.tag[index] }}</p>
        </div>
        <div class="card-hover d-none card-body">
            <div class="top-right">
                <div>hej</div>
                <div>på</div>
                <div>dig</div>
            </div>
            <div class="bottom-left">
                på dig
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
        background-color: white;
        border-radius: 20px;
        padding: 5px;
        margin: 5px;
    }

    .bottom-left {
        position:absolute;
        bottom: 0px;
        left: 0px;
    }

    .card-main {
        position: relative;
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