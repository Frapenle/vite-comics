<script>
import HeaderVue from "./components/HeaderVue.vue";
import MainVue from "./components/MainVue.vue";
import FooterVue from "./components/FooterVue.vue";

export default {
  components: {
    HeaderVue,
    MainVue,
    FooterVue
  }
}
</script>

<template>
  <div class="container">

    <HeaderVue />
    <MainVue />
    <FooterVue />
  </div>

</template>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.container {
  max-width: 980px;
  margin: 0 auto;
  padding: 0 50px;
}
</style>
