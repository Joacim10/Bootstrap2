<template>
    <div class="row mx-2">
        <div class="col-sm-3">
            <div class="card">
                <div class="d-flex justify-content-between card-body align-items-center">
                    <div class="mr-3">
                        <img class="" src="@/assets/box.png" alt="">
                    </div>
                    <div class="">
                        <h5 class="card-title text-info">Free shipping</h5>
                        <p class="card-text t-small">For a local customer, we provide free shipping facility</p>
                    </div>
                </div>
            </div>
        </div>

        <div class="col-sm-3">
            <div class="card">
                <div class="d-flex justify-content-between card-body align-items-center">
                    <div class="mr-3">
                        <img class="" src="@/assets/box.png" alt="">
                    </div>
                    <div class="">
                        <h5 class="card-title text-info">Free shipping</h5>
                        <p class="card-text t-small">For a local customer, we provide free shipping facility</p>
                    </div>
                </div>
            </div>
        </div>

        <div class="col-sm-3">
            <div class="card">
                <div class="d-flex justify-content-between card-body align-items-center">
                    <div class="mr-3">
                        <img class="" src="@/assets/box.png" alt="">
                    </div>
                    <div class="">
                        <h5 class="card-title text-info">Free shipping</h5>
                        <p class="card-text t-small">For a local customer, we provide free shipping facility</p>
                    </div>
                </div>
            </div>
        </div>

        <div class="col-sm-3">
            <div class="card">
                <div class="d-flex justify-content-between card-body align-items-center">
                    <div class="mr-3">
                        <img class="" src="@/assets/box.png" alt="">
                    </div>
                    <div class="">
                        <h5 class="card-title text-info">Free shipping</h5>
                        <p class="card-text t-small">For a local customer, we provide free shipping facility</p>
                    </div>
                </div>
            </div>
        </div>

    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
    .card {
        border: 0;
        background-color: rgb(32, 213, 195, 0.08);
    }

    .card:hover {
        border: 0;
        background-color: rgba(32, 213, 195, 1);
        color: white;
    }

    .card > div > div > h5 {
        font-size: 1rem;
        font-weight: 300;
    }

    .card:hover > div > div > h5 {
        color: white !important;
    }

    .card:hover > div > div > img {
        -webkit-filter: grayscale(100%); /* Safari 6.0 - 9.0 */
        filter: grayscale(100%) brightness(200%);
    }



</style>