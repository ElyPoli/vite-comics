<script>
export default {

};
</script>

<template>
    <div class="banner pt-4 pb-4 overflow-hidden">
        <div class="row justify-content-center">
            <div class="col-12 col-sm-6 col-md-4 col-lg-2">
                <div class="d-flex align-items-center justify-content-center">
                    <img src="/public/img/buy-comics-digital-comics.png" alt="digital comics" class="pe-2">
                    <p class="text-white text-uppercase text-nowrap m-0 p-0">digital comics</p>
                </div>
            </div>
            <div class="col-12 col-sm-6 col-md-4 col-lg-2">
                <div class="d-flex align-items-center justify-content-center pt-sm-0 pt-4">
                    <img src="/public/img/buy-comics-merchandise.png" alt="merchandise" class="pe-2">
                    <p class="text-white text-uppercase text-nowrap m-0 p-0">dc merchandise</p>
                </div>
            </div>
            <div class="col-12 col-sm-6 col-md-4 col-lg-2">
                <div class="d-flex align-items-center justify-content-center pt-md-0 pt-sm-4 pt-4">
                    <img src="/public/img/buy-comics-subscriptions.png" alt="subscriptions" class="pe-2">
                    <p class="text-white text-uppercase text-nowrap m-0 p-0">subscriptions</p>
                </div>
            </div>
            <div class="col-12 col-sm-6 col-md-4 col-lg-2">
                <div class="d-flex align-items-center justify-content-center pt-lg-0 pt-sm-4 pt-4">
                    <img src="/public/img/buy-comics-shop-locator.png" alt="shop locator" class="pe-2">
                    <p class="text-white text-uppercase text-nowrap m-0 p-0">comic shop locator</p>
                </div>
            </div>
            <div class="col-12 col-sm-6 col-md-4 col-lg-2">
                <div class="d-flex align-items-center justify-content-center pt-lg-0 pt-sm-4 pt-4">
                    <img src="/public/img/buy-dc-power-visa.svg" alt="power visa" class="pe-2">
                    <p class="text-white text-uppercase text-nowrap m-0 p-0">dc power visa</p>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

.banner {
    background-color: $primary-color;

    img {
        max-width: 100%;
        max-height: 40px;
        height: auto;
    }

    p {
        font-size: .8rem;
    }
}
</style>
