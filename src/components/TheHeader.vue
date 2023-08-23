<script>
export default {
    data() {
        return {
            headerNav: [
                "characters",
                "comics",
                "movies",
                "tv",
                "games",
                "collectibles",
                "videos",
                "fans",
                "news",
                "shop",
            ]
        };
    }
};
</script>

<template>
    <header class="container d-flex align-items-center justify-content-between pt-4 pb-4 overflow-hidden">
        <!-- Logo -->
        <div>
            <a href="#" class="my-navbar-logo">
                <img src="/public/img/dc-logo.png" alt="DC logo">
            </a>
        </div>

        <!-- Menù -->
        <nav class="ps-2 ps-sm-4 ps-md-0">
            <ul class="my-navbar-link d-flex flex-wrap align-items-center justify-content-center">
                <li class="list-group-item pt-1 pt-md-0" v-for="navLink in headerNav">
                    <a href="#" class="link-underline link-underline-opacity-0"> {{ navLink }} </a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

.my-navbar-logo {
    img {
        max-width: 5rem;
    }
}

.my-navbar-link {
    display: flex;
    flex-direction: row;
    padding-left: 0;
    margin-bottom: 0;

    .list-group-item {
        padding: 0 1rem;
        text-transform: uppercase;
        font-size: .8rem;
        font-weight: bold;

        a {
            color: $secondary-color;
            transition: color .2s;
        }

        a:hover {
            color: $primary-color;
        }
    }
}
</style>
