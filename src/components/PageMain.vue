<template>
  <main>
    <div class="jumbo"></div>
    <div class="container">
      <div class="content">
        <h2> Content goes here </h2>
      </div>
    </div>
  </main>
</template>

<script>

export default {
  name: "PageMain",
};
</script>

<style scoped lang="scss">
@import "../assets/style/partials/variables.scss";

main {
  background: #1c1c1c;
  min-height: 120px;
  justify-content: center;
  display: flex;
}
</style>
