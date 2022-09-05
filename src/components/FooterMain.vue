<template>
  <footer>
    <FooterTop />
    <FooterMid />
    <FooterBot />
  </footer>
</template>

<script>
import FooterTop from "./FooterTop.vue";
import FooterMid from "./FooterMid.vue";
import FooterBot from "./FooterBot.vue";

export default {
  name: "FooterMain",
  components: {
    FooterTop,
    FooterMid,
    FooterBot,
  },
};
</script>

<style scoped lang="scss">
@import "../assets/style/partials/variables.scss";
</style>
