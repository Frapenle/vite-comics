<script>
import HeaderVue from "./components/HeaderVue.vue";
import HeroImage from "./components/HeroImage.vue";
import MainVue from "./components/MainVue.vue";
import FooterVue from "./components/FooterVue.vue";

export default {
  components: {
    HeaderVue,
    HeroImage,
    MainVue,
    FooterVue
  }
}
</script>

<template>
  <HeaderVue />
  <HeroImage />
  <MainVue />
  <FooterVue />
</template>

<style lang="scss">
@use "./styles/general.scss" as *;
@use "./styles/partials/variables" as *;
</style>
