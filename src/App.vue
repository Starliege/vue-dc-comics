<template>
  <div id="app">
    <PageHeader />
    <PageMain />
    <FooterMain />
  </div>
</template>

<script>
import FooterMain from "./components/FooterMain.vue";
import PageHeader from "./components/PageHeader.vue";
import PageMain from "./components/PageMain.vue";

export default {
  name: "App",
  components: {
    FooterMain,
    PageHeader,
    PageMain
},
};
</script>

<style lang="scss">
@import "./assets/style/global.scss";
</style>
