<script>
export default {
    props: {
        thumb: String,
        price: String,
        series: String,
        type: String,
    }
}
</script>

<template>
    <div class="comics-list pt-3 d-flex justify-content-center">
        <div>
            <img v-bind:src="thumb" v-bind:alt="series">
            <p class="text-white text-uppercase m-0 p-0 pt-2"> {{ series }} </p>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

.comics-list {
    cursor: pointer;

    img {
        height: 135px;
        width: 120px;
        object-fit: cover;
        object-position: top;
        transition: filter 0.3s;
    }

    p {
        font-size: .8rem;
        width: 120px;
    }
}

.comics-list:hover {
    img {
        filter: brightness(0.6);
    }
}
</style>
