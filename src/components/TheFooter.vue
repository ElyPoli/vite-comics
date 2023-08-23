<script>
export default {
    data() {
        return {
            footerNav: [
                {
                    dcComics: [
                        "Characters",
                        "Comics",
                        "Movies",
                        "TV",
                        "Games",
                        "Videos",
                        "News",
                    ],
                },
                {
                    shop: [
                        "Shop DC",
                        "Shop DC collectibles",
                    ],
                },
                {
                    dc: [
                        "Terms Of Use",
                        "Privacy policy (New)",
                        "Ad Choices",
                        "Advertising",
                        "Jobs",
                        "Subscriptions",
                        "Talent Workshops",
                        "CPSC Certificates",
                        "Ratings",
                        "Shop Help",
                        "Contact Us",
                    ],
                },
                {
                    sites: [
                        "DC",
                        "MAD Magazine",
                        "DC Kids",
                        "DC Universe",
                        "DC Power Visa",
                    ],
                },
            ],
        };
    },
}
</script>

<template>
    <footer>
        <!-- Sezione superiore del footer -->
        <div class="top-footer">
            <div class="container d-flex align-items-start justify-content-between">
                <!-- Menù -->
                <div class="d-flex align-items-start justify-content-between pb-3">
                    <div class="pe-4">
                        <h3 class="text-uppercase text-white text-nowrap fw-bold fs-6 m-0 p-0 pt-4 pb-3">DC comics</h3>
                        <p v-for="navLink in footerNav[0].dcComics"> {{ navLink }} </p>
                        <h3 class="text-uppercase text-white text-nowrap fw-bold fs-6 m-0 p-0 pt-4 pb-3">Shop</h3>
                        <p v-for="navLink in footerNav[1].shop"> {{ navLink }} </p>
                    </div>
                    <div class="pe-4 ps-4">
                        <h3 class="text-uppercase text-white text-nowrap fw-bold fs-6 m-0 p-0 pt-4 pb-3">DC</h3>
                        <p v-for="navLink in footerNav[2].dc"> {{ navLink }} </p>
                    </div>
                    <div class="ps-4">
                        <h3 class="text-uppercase text-white text-nowrap fw-bold fs-6 m-0 p-0 pt-4 pb-3">Sites</h3>
                        <p v-for="navLink in footerNav[3].sites"> {{ navLink }} </p>
                    </div>
                </div>
                <!-- Logo -->
                <img class="footer-logo" src="/public/img/dc-logo-bg.png" alt="DC logo">
            </div>
        </div>

        <!-- Sezione inferiore del footer -->
        <div class="bottom-footer pt-4 pb-4">
            <div class="container">
                <div class="row align-items-center justify-content-between">
                    <!-- Pulsante -->
                    <div class="col-12 col-md-6">
                        <div class="my-social d-flex align-items-center justify-content-center">
                            <button type="button" class="btn my-btn-footer text-uppercase">
                                sing-up now!
                            </button>
                        </div>
                    </div>
                    <!-- Social -->
                    <div class="col-12 col-md-6">
                        <div class="my-social d-flex align-items-center justify-content-center pt-md-0 pt-4">
                            <p class="m-0 p-0 text-uppercase text-nowrap ps-4">Follow us</p>
                            <img src="/public/img/footer-fb.png" alt="Facebook">
                            <img src="/public/img/footer-tw.png" alt="Twitter">
                            <img src="/public/img/footer-youtube.png" alt="Youtube">
                            <img src="/public/img/footer-pinterest.png" alt="Pinterest">
                            <img src="/public/img/footer-periscope.png" alt="Periscope">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

.top-footer {
    background-image: url("/public/img/footer-bg.jpg");
    height: 380px;
    overflow: hidden;

    p {
        padding: 0 0 .2rem 0;
        margin: 0;
        font-size: .8rem;
        color: #999797;
        cursor: pointer;
    }

    p:hover {
        text-decoration: underline;
    }
}

.footer-logo {
    margin-top: -93px;
}

.bottom-footer {
    background-color: $secondary-color;
}

.my-btn-footer {
    color: #ffffff;
    border: 2px solid $primary-color;
    border-radius: 0%;
    transition: background-color .2s;
}

.my-btn-footer:hover {
    background-color: $primary-color;
}

.my-social {
    p {
        color: $primary-color;
        font-weight: bold;
        font-size: 1.2rem;
        padding: 0 1rem;
    }

    img {
        padding: 0 .5rem;
        cursor: pointer;
        transition: transform .2s;
    }

    img:hover {
        transform: scale(.93);
    }

}
</style>
