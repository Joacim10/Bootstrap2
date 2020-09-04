<template>
<div>
   <div class="card-carousel-wrapper">
    <div class="card-carousel--nav__left" @click="moveCarousel(-1)" :disabled="atHeadOfList"></div>
    <div class="card-carousel">
      <div class="card-carousel--overflow-container">
        <div class="card-carousel-cards" :style="{ transform: 'translateX' + '(' + currentOffset + '%' + ')' }">
            <Card class="card-carousel--card" :style="computedWidthAndMargin" v-for="item in items" :key="item.name" :item="item" :name="item.name" :tag="items.tag" />
        </div>
      </div>
    </div>
    <div class="card-carousel--nav__right" @click="moveCarousel(1)" :disabled="atEndOfList"></div>
  </div>
</div>
</template>

<script>
import Card from '@/components/card.vue'


export default {
  components: {
    Card
  },
  props: ['windowSize', 'items'],  
data() {
    return {
      currentOffset: 0,
      paginationFactor: Number,
      cardWidth: Number,
      cardMargin: Number
    }
  },
  computed: {
    computedWidthAndMargin() {
      return {
        "min-width": `${this.cardWidth}%`,
        "margin-right": `${this.cardMargin}%`
      };      
    },
    atEndOfList() {
      return this.currentOffset <= (this.paginationFactor * -1) * (this.items.length - this.windowSize);
    },
    atHeadOfList() {
      return this.currentOffset === 0;
    },
  },
  methods: {
    moveCarousel(direction) {
      // Find a more elegant way to express the :style. consider using props to make it truly generic
      if (direction === 1 && !this.atEndOfList) {
        this.currentOffset -= this.paginationFactor;
      } else if (direction === -1 && !this.atHeadOfList) {
        this.currentOffset += this.paginationFactor;
      }
    },
  },
  mounted: function() {
      this.cardMargin = 6/this.windowSize
      this.cardWidth = (100 - (this.cardMargin * (this.windowSize - 1))) / this.windowSize
      this.paginationFactor = +((this.cardWidth + this.cardMargin).toFixed(2))
      console.log(this.items)
  }
}
</script>

<style scoped>
body {
  background: #f8f8f8;
  color: #2c3e50;
  font-family: 'Source Sans Pro', sans-serif;
}

.card-carousel-wrapper {
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 20px 0 40px;
  color: #666a73;
  width: 100%;
}

/deep/ .card-carousel {
  display: flex;
  justify-content: center;
  width: 100%;
}
.card-carousel--overflow-container {
  overflow: hidden;
  width: 100%;
}
.card-carousel--nav__left, .card-carousel--nav__right {
  display: inline-block;
  width: 15px;
  height: 15px;
  padding: 10px;
  box-sizing: border-box;
  border-top: 2px solid #42b883;
  border-right: 2px solid #42b883;
  cursor: pointer;
  margin: 0 20px;
  transition: transform 150ms linear;
}
.card-carousel--nav__left[disabled], .card-carousel--nav__right[disabled] {
  opacity: 0.2;
  border-color: black;
}
.card-carousel--nav__left {
  transform: rotate(-135deg);
}
.card-carousel--nav__left:active {
  transform: rotate(-135deg) scale(0.9);
}
.card-carousel--nav__right {
  transform: rotate(45deg);
}
.card-carousel--nav__right:active {
  transform: rotate(45deg) scale(0.9);
}

.card-carousel-cards {
  width: 100%;
  display: flex;
  transition: transform 150ms ease-out;
  transform: translatex(0px);
}
/deep/ .card-carousel-cards .card-carousel--card {
  margin-right: 3%;
  cursor: pointer;
  box-shadow: 0 4px 15px 0 rgba(40, 44, 53, 0.06), 0 2px 2px 0 rgba(40, 44, 53, 0.08);
  border-radius: 4px;
  z-index: 3;
  margin-bottom: 2px;
/*   width: 31.333%;
 */}

/deep/ .card-carousel-cards .card-carousel--card:first-child {
  margin-left: 0;
}
/deep/ .card-carousel-cards .card-carousel--card:last-child {
  margin-right: 0;
}
/deep/ .card-carousel-cards .card-carousel--card img {
  vertical-align: bottom;
  border-top-left-radius: 4px;
  border-top-right-radius: 4px;
  transition: opacity 150ms linear;
  user-select: none;
}
/deep/ .card-carousel-cards .card-carousel--card img:hover {
  opacity: 0;
  
}
/deep/ .card-carousel-cards .card-carousel--card--footer {
  border-top: 0;
  padding: 7px 15px;
}
/deep/ .card-carousel-cards .card-carousel--card--footer p {
  padding: 3px 0;
  margin: 0;
  margin-bottom: 2px;
  font-size: 19px;
  font-weight: 500;
  color: #2c3e50;
  user-select: none;
}
/deep/ .card-carousel-cards .card-carousel--card--footer p.tag {
  font-size: 11px;
  font-weight: 300;
  padding: 4px;
  background: rgba(40, 44, 53, 0.06);
  display: inline-block;
  position: relative;
  margin-left: 4px;
  color: #666a73;
}
/* /deep/ .card-carousel-cards .card-carousel--card--footer p.tag:before {
  content: "";
  float: left;
  position: absolute;
  top: 0;
  left: -12px;
  width: 0;
  height: 0;
  border-color: transparent rgba(40, 44, 53, 0.06) transparent transparent;
  border-style: solid;
  border-width: 8px 12px 12px 0;
} */
/deep/ .card-carousel-cards .card-carousel--card--footer p.tag.secondary {
  margin-left: 0;
  border-left: 1.45px dashed white;
}
/deep/ .card-carousel-cards .card-carousel--card--footer p.tag.secondary:before {
  display: none !important;
}
/* /deep/ .card-carousel-cards .card-carousel--card--footer p.tag:after {
  content: "";
  position: absolute;
  top: 8px;
  left: -3px;
  float: left;
  width: 4px;
  height: 4px;
  border-radius: 2px;
  background: white;
  box-shadow: -0px -0px 0px #004977;
} */

h1 {
  font-size: 3.6em;
  font-weight: 100;
  text-align: center;
  margin-bottom: 0;
  color: #42b883;
}

</style>