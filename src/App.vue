<script>
import TheHeader from './components/TheHeader.vue';
import TheFooter from './components/TheFooter.vue';
import IndexBanner from './components/IndexBanner.vue';
import CurrentSeries from './components/CurrentSeries.vue';
import comics from './db/comics';

export default {
  components: {
    TheHeader,
    TheFooter,
    IndexBanner,
    CurrentSeries,
  },
  data() {
    return {
      comics,
    }
  },
}
</script>

<template>
  <TheHeader></TheHeader>
  <main class="comics-main">
    <img src="/public/img/jumbotron.jpg" alt="bg image" class="my-jumbotron">
    <div class="container pb-3">
      <div class="section-comics-title">
        <h3 class="text-uppercase p-0 m-0 fs-5">
          current series
        </h3>
      </div>
      <div class="row">
        <div class="col-6 col-sm-4 col-md-3 col-lg-2" v-for="(comicSingle, i) in comics" :key="`comicSingle_${i}`">
          <CurrentSeries v-bind:thumb="comicSingle.thumb" v-bind:series="comicSingle.series">
          </CurrentSeries>
        </div>
      </div>
      <div class="d-flex align-items-center justify-content-center pt-2">
        <button type="button" class="btn my-btn-comics text-uppercase pe-5 ps-5">
          load more
        </button>
      </div>
    </div>
  </main>
  <IndexBanner></IndexBanner>
  <TheFooter></TheFooter>
</template>

<style lang="scss" scoped>
@use "styles/partials/variables" as *;

.comics-main {
  background-color: #1c1c1c;
}

.my-jumbotron {
  max-height: 300px;
  width: 100%;
  object-fit: cover;
  object-position: top;
}

.section-comics-title {
  background-color: $primary-color;
  padding: .7rem;
  text-align: center;
  width: 200px;
  margin-top: -25px;
  margin-bottom: 1rem;
  position: relative;
  z-index: 5;

  h3 {
    color: #ffffff;
    font-weight: bold;
  }
}

.my-btn-comics {
  color: #ffffff;
  background-color: $primary-color;
  border: 2px solid $primary-color;
  border-radius: 0%;
  transition: transform .3s;
  font-weight: bold;
  font-size: .8rem;
}

.my-btn-comics:hover {
  transform: scale(.97);
}
</style>
