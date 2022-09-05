<template>
  <header>
    <div class="container">
      <a href="#"><img src="../assets/img/dc-logo.png" alt="DC" /></a>
      <nav>
        <ul>
          <li v-for="(link, index) in menuArr" :key="index">
            <a :href="link.link" :class="{ active: link.active }">{{
              link.name
            }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "PageHeader",
  data() {
    return {
      menuArr: [
        {
          name: "Characters",
          link: "#",
          active: false,
        },
        {
          name: "Comics",
          link: "#",
          active: true,
        },
        {
          name: "Movies",
          link: "#",
          active: false,
        },
        {
          name: "TV",
          link: "#",
          active: false,
        },
        {
          name: "Games",
          link: "#",
          active: false,
        },
        {
          name: "Collectibles",
          link: "#",
          active: false,
        },
        {
          name: "Videos",
          link: "#",
          active: false,
        },
        {
          name: "Fans",
          link: "#",
          active: false,
        },
        {
          name: "News",
          link: "#",
          active: false,
        },
        {
          name: "Shop",
          link: "#",
          active: false,
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets/style/partials/variables.scss";

header {
  background: #fff;

  img {
    margin: 11px 0;
  }
}

nav {
  font-family: "Roboto Condensed", sans-serif;
  text-transform: uppercase;
  display: inline-block;

  ul {
    list-style-type: none;

    li {
      display: inline-block;
      margin: 0 20px;

      a {
        padding: 50px 0;
        color: #464645;
        text-decoration: none;
      }

      .active {
        border-bottom: 5px solid $accent;
      }
    }
  }
}
</style>
