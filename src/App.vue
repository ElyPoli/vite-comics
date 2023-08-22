<script>
import TheHeader from './components/TheHeader.vue';
import TheFooter from './components/TheFooter.vue';
import IndexBanner from './components/IndexBanner.vue';

export default {
  components: {
    TheHeader,
    TheFooter,
    IndexBanner,
  },
  data() {
    return {}
  },
}
</script>

<template>
  <TheHeader></TheHeader>
  <main class="index-main pt-4 pb-4">
    <div class="container">
      <p class="text-white fw-bold fs-5 m-0 p-0">&lt;-- Content goes here --&gt;</p>
    </div>
  </main>
  <IndexBanner></IndexBanner>
  <TheFooter></TheFooter>
</template>

<style></style>
