<script>
export default {

};
</script>

<template>
    <div class="banner">
        <div class="container pt-5 pb-5 d-flex align-items-center justify-content-around">
            <div class="d-flex align-items-center justify-content-around">
                <img src="/public/img/buy-comics-digital-comics.png" alt="digital comics" class="pe-4">
                <p class="text-white text-uppercase m-0 p-0">digital comics</p>
            </div>
            <div class="d-flex align-items-center justify-content-around">
                <img src="/public/img/buy-comics-merchandise.png" alt="merchandise" class="pe-4">
                <p class="text-white text-uppercase m-0 p-0">dc merchandise</p>
            </div>
            <div class="d-flex align-items-center justify-content-around">
                <img src="/public/img/buy-comics-subscriptions.png" alt="subscriptions" class="pe-4">
                <p class="text-white text-uppercase m-0 p-0">subscriptions</p>
            </div>
            <div class="d-flex align-items-center justify-content-around">
                <img src="/public/img/buy-comics-shop-locator.png" alt="shop locator" class="pe-4">
                <p class="text-white text-uppercase m-0 p-0">comic shop locator</p>
            </div>
            <div class="d-flex align-items-center justify-content-around">
                <img src="/public/img/buy-dc-power-visa.svg" alt="power visa" class="pe-4">
                <p class="text-white text-uppercase m-0 p-0">dc power visa</p>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

.banner {
    background-color: $primary-color;

    img {
        height: 50px;
    }
}

</style>
