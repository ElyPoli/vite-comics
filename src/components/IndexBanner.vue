<script>
export default {
    data() {
        return {
            bannerList: [
                {
                    name: "digital comics",
                    srcImg: "/public/img/buy-comics-digital-comics.png",
                },
                {
                    name: "dc merchandise",
                    srcImg: "/public/img/buy-comics-merchandise.png",
                },
                {
                    name: "subscriptions", 
                    srcImg: "/public/img/buy-comics-subscriptions.png",
                },
                {
                    name: "comic shop locator", 
                    srcImg: "/public/img/buy-comics-shop-locator.png",
                },
                {
                    name: "dc power visa", 
                    srcImg: "/public/img/buy-dc-power-visa.svg",
                },
            ],
        };
    },
};
</script>

<template>
    <div class="banner pt-4 pb-4 overflow-hidden">
        <div class="row justify-content-center">
            <div class="col-12 col-sm-6 col-md-4 col-lg-2" v-for="banner in bannerList">
                <div class="d-flex align-items-center justify-content-center">
                    <img v-bind:src="banner.srcImg" v-bind:alt="banner.name" class="pe-2">
                    <p class="text-white text-uppercase text-nowrap m-0 p-0"> {{ banner.name }} </p>
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
