<script>
import AppTitle from "./components/AppTitle.vue";
import AppBanner from "./components/AppBanner.vue";
export default {
  components: {
    AppTitle,
    AppBanner,
  },
};
</script>

<template>
  <h1 class="title text-center">Hello</h1>

  <AppBanner />

  <AppTitle />

  <h2>Altro h2</h2>
</template>

<style>
.text-center {
  text-align: center;
}

.title {
  color: green;
}
</style>
