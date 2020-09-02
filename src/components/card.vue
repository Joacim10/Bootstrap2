<template>
    <div class="card-main">
        <div class="card-original">
            <img src="https://placehold.it/200x200"/>
            <div class="card-carousel--card--footer card-body">
                <p>{{ item.name }}</p>
                <p class="tag" v-for="(tag,index) in item.tag" :key="tag" :class="index &gt; 0 ? 'secondary' : ''">{{ item.tag[index] }}</p>
            </div>
        </div>
        <div class="card-hover d-none">
            <img class="img" src="https://placehold.it/200x200"/>
            <div class="card-carousel--card--footer card-body">
                <p>{{ item.name }}</p>
                <p class="tag" v-for="(tag,index) in item.tag" :key="tag" :class="index &gt; 0 ? 'secondary' : ''">{{ item.tag[index] }}</p>
                <p>150$</p>
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
    .card-body{
        background-color: #0E153D;
    }
    .card-main:hover > .card-original {
        display: none;
    }
    .card-main:hover > .card-hover {
        display: block !important;
    }

    .card-hover {
        background-color: #0E153D;
    }

</style>