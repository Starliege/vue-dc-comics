<template>
  <main>
    <div class="jumbo"></div>
    <div class="container">
      <div class="content">
        <h2>Current Series</h2>
        <ComicProduct
          v-for="(element, index) in comicsArr"
          :key="index"
          :comic="element"
        />
      </div>
      <a href="#" class="load-more">Load more</a>
    </div>
  </main>
</template>

<script>
import ComicsData from "../assets/data/dc-comics.json";
import ComicProduct from "./commons/ComicProduct.vue";

export default {
  name: "PageMain",
  components: {
    ComicProduct
},
  data() {
    return {
      comicsArr: ComicsData,
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets/style/partials/variables.scss";

main {
  background: #1c1c1c;

  .jumbo {
    height: 500px;
    width: 100%;
    background: url("../assets/img/jumbotron.jpg");
    background-size: cover;
  }

  .container {
    position: relative;
    display: block;
    text-align: center;
    padding-bottom: 100px;

    .content {
      width: 100%;
      padding: 100px 0;
      display: flex;
      align-items: flex-start;
      flex-wrap: wrap;
      gap: 100px 50px;

      h2 {
        position: absolute;
        top: -25px;
        left: -25px;
        padding: 10px 25px;
        width: fit-content;
        background: $accent;
        text-transform: uppercase;
      }
    }

    a.load-more {
      padding: 15px 70px;
      width: max-content;
      background: $accent;
      font-family: "Roboto Condensed", sans-serif;
      font-size: 1.5rem;
      text-transform: uppercase;
      text-decoration: none;
      color: #fff;

      &:hover {
        background: #1990ff;
      }
    }
  }
}
</style>

