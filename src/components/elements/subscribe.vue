<template>
    <div class="bg-light-grey my-4">
        <div class="container d-flex justify-content-between text-center text-md-left">
            <div class="my-5">
                <h2 class="d-inline-block">SUBSCRIBE <h2 class="text-info d-inline-block"> NOW </h2></h2>
                <p class="w-md-75">Signup for awesome news about our new products and know our special discounts on products.</p>
                <form id="form" action="">
                    <input class="rounded" type="text" placeholder="Enter email address">
                    <button class="btn rounded btn-info">Subscribe</button>
                </form>
            </div>
            <div class="d-none d-md-block bg-grey w-100">
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>

form {
    width: 100%;
    position: relative;
    padding-right: 10px;
}

input {
    padding: 10px;
    margin: 0;
    width: 100%;
    border: 1px solid #c7c7c7;
}

input::placeholder {
    color: #c7c7c7;
}

.btn {
    position: absolute;
    right: 15px;
    margin: 0;
    top: 5px;
    border: none;
}

</style>