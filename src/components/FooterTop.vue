<template>
  <section>
    <div class="container">
      <nav>
        <ul>
          <li v-for="(link, index) in menuArr" :key="index">
            <a href="#">
              <img :src="link.img" :alt="link.text" />
              <span>{{ link.text }}</span>
            </a>
          </li>
        </ul>
      </nav>
    </div>
  </section>
</template>

<script>
export default {
  name: "FooterTop",
  data() {
    return {
      menuArr: [
        {
          text: "Digital Comics",
          img: require("../assets/img/buy-comics-digital-comics.png"),
        },
        {
          text: "DC Merchandise",
          img: require("../assets/img/buy-comics-merchandise.png"),
        },
        {
          text: "Subscription",
          img: require("../assets/img/buy-comics-subscriptions.png"),
        },
        {
          text: "Comic Shop Locator",
          img: require("../assets/img/buy-comics-shop-locator.png"),
        },
        {
          text: "DC Power Visa",
          img: require("../assets/img/buy-dc-power-visa.svg"),
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets/style/partials/variables.scss";

section {
  padding: 30px 0;
  background: $accent;

  .container {
    justify-content: center;

    ul {
      list-style: none;
      display: flex;
      align-items: center;
      gap: 50px;

      li {
        a {
          display: flex;
          align-items: center;
          gap: 30px;
          color: #fff;
          font-weight: normal;
          text-decoration: none;
          text-transform: uppercase;

          span {
            width: max-content;
            white-space: nowrap;
          }

          img {
            max-height: 50px;
          }
        }
      }
    }
  }
}
</style>
