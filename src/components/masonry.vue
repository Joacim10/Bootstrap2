<template>
    <div class="grid-layout text-info my-5">
        <div class="grid-item grid-item-1">
            <div class="bottom-label">Men</div>
        </div>
        <div class="grid-item span-2-1 grid-item-2">
            <div class="bottom-label">Women</div>
        </div>
        <div class="grid-item span-2-2 grid-item-3">
            <div class="bottom-label">Kids</div>
        </div>
        <div class="grid-item span-2-2 grid-item-4">
            <div class="bottom-label">Shoes</div>
        </div>
        <div class="grid-item span-2 grid-item-5">
            <div class="bottom-label">Hats</div>
        </div>
        <div class="grid-item span-2-1 grid-item-6">
            <div class="bottom-label">Sunglasses

            <div class="text-white small">18 products</div> 
            </div>
        </div>
        <div class="grid-item grid-item-7">
            <div class="bottom-label">Watches</div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>

.bottom-label {
    position: absolute;
    left: 0;
    bottom: 0;
    z-index: +1;
    width: 50%;
    background-color: #0E153D;
    padding: 5px;
}

.grid-layout {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(180px, 1fr));
    grid-gap: 10px;
    grid-auto-rows: minmax(180px, auto);
    grid-auto-flow: dense;
    padding: 10px;
}

.grid-item {
    position: relative;
    padding: 1rem;
    font-size: 14px;
    font-weight: bold;
    background-color: #CCCCCC;
    border-radius: 5px;
}

.span-2-2 {
    grid-column-end: span 2;
    grid-row-end: span 2;
}

.span-2-1 {
    grid-column-end: span 2;
    grid-row-end: span 1;
}
</style>