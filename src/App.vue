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
  <main class="comics-main pt-5 pb-3">
    <div class="container">
      <div class="row">
        <div class="col-6 col-sm-4 col-md-3 col-lg-2" v-for="(comicSingle, i) in comics" :key="`comicSingle_${i}`">
          <CurrentSeries v-bind:thumb="comicSingle.thumb" v-bind:series="comicSingle.series">
          </CurrentSeries>
        </div>
      </div>
      <div class="d-flex align-items-center justify-content-center pt-2">
        <button type="button" class="btn my-btn-comics text-uppercase">
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

.my-btn-comics {
  color: #ffffff;
  background-color: $primary-color;
  border: 2px solid $primary-color;
  border-radius: 0%;
  transition: scale .2s;
  font-weight: bold;
  font-size: .8rem;
}

.my-btn-comics:hover {
  transform: scale(.95);
}
</style>
