<script>
export default {

}
</script>

<template>
    <header class="container d-flex align-items-center justify-content-between pt-4 pb-4">
        <!-- Logo -->
        <div>
            <a href="#" class="my-navbar-logo">
                <img src="/public/img/dc-logo.png" alt="DC logo">
            </a>
        </div>

        <!-- Menù -->
        <nav>
            <ul class="my-navbar-link">
                <li class="list-group-item">
                    <a href="#" class="link-underline link-underline-opacity-0">characters</a>
                </li>
                <li class="list-group-item">
                    <a href="#" class="link-underline link-underline-opacity-0">comics</a>
                </li>
                <li class="list-group-item">
                    <a href="#" class="link-underline link-underline-opacity-0">movies</a>
                </li>
                <li class="list-group-item">
                    <a href="#" class="link-underline link-underline-opacity-0">tv</a>
                </li>
                <li class="list-group-item">
                    <a href="#" class="link-underline link-underline-opacity-0">games</a>
                </li>
                <li class="list-group-item">
                    <a href="#" class="link-underline link-underline-opacity-0">collectibles</a>
                </li>
                <li class="list-group-item">
                    <a href="#" class="link-underline link-underline-opacity-0">videos</a>
                </li>
                <li class="list-group-item">
                    <a href="#" class="link-underline link-underline-opacity-0">fans</a>
                </li>
                <li class="list-group-item">
                    <a href="#" class="link-underline link-underline-opacity-0">news</a>
                </li>
                <li class="list-group-item">
                    <a href="#" class="link-underline link-underline-opacity-0">shop</a>
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
            color: $link-color;
            transition: color .2s;
        }

        a:hover {
            color: $link-color-hover;
        }
    }
}
</style>
