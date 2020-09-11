<template>
<div id="fourCards" class="mx-lg-4">
    <div class="row mx-2">
        <div class="col-12 col-sm-6 col-md-4 col-lg-3 p-1">
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

        <div class="col-12 col-sm-6 col-md-4 col-lg-3 p-1">
            <div class="card">
                <div class="d-flex justify-content-between card-body align-items-center">
                    <div class="mr-3">
                        <img class="" src="@/assets/icon2.png" alt="">
                    </div>
                    <div class="">
                        <h5 class="card-title text-info">24/7 support</h5>
                        <p class="card-text t-small">For any inquiry, we are available 24 hours every day</p>
                    </div>
                </div>
            </div>
        </div>

        <div class="col-12 col-sm-6 col-md-4 col-lg-3 p-1">
            <div class="card">
                <div class="d-flex justify-content-between card-body align-items-center">
                    <div class="mr-3">
                        <img class="" src="@/assets/icon3.png" alt="">
                    </div>
                    <div class="">
                        <h5 class="card-title text-info">Online payment</h5>
                        <p class="card-text t-small">You can pay quickly and easily with our online payment system</p>
                    </div>
                </div>
            </div>
        </div>

        <div class="col-12 col-sm-6 d-md-none d-lg-block col-lg-3 p-1">
            <div class="card">
                <div class="d-flex justify-content-between card-body align-items-center">
                    <div class="mr-3">
                        <img class="" src="@/assets/icon4.png" alt="">
                    </div>
                    <div class="">
                        <h5 class="card-title text-info">Fast delivery</h5>
                        <p class="card-text t-small">We understand your urgency and we deliver in a fast way</p>
                    </div>
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

    #fourCards {
        display: flex;
        justify-content: center;
    }

    .row {
        max-width: 1400px;
    }

    .card {
        border: 0;
        background-color: rgb(32, 213, 195, 0.08);
        height: 100%;
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