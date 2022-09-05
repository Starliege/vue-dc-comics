<template>
  <section>
    <div class="container">
      <nav>
        <div>
          <h3>DC Comics</h3>
          <ul>
            <li>
              <a href="#">Characters</a>
            </li>
            <li>
              <a href="#">Comics</a>
            </li>
            <li>
              <a href="#">Movies</a>
            </li>
            <li>
              <a href="#">TV</a>
            </li>
            <li>
              <a href="#">Games</a>
            </li>
            <li>
              <a href="#">Videos</a>
            </li>
            <li>
              <a href="#">News</a>
            </li>
          </ul>

          <h3>Shop</h3>
          <ul>
            <li>
              <a href="#">Shop DC</a>
            </li>
            <li>
              <a href="#">Shop DC Collectibles</a>
            </li>
          </ul>
        </div>
        <div>
          <h3>DC</h3>
          <ul>
            <li>
              <a href="#">Terms of use</a>
            </li>
            <li>
              <a href="#">Privacy policy (new)</a>
            </li>
            <li>
              <a href="#">Ad choises</a>
            </li>
            <li>
              <a href="#">Advertising</a>
            </li>
            <li>
              <a href="#">Jobs</a>
            </li>
            <li>
              <a href="#">Subscriptions</a>
            </li>
            <li>
              <a href="#">Talent Workshops</a>
            </li>
            <li>
              <a href="#">CPSC Certificates</a>
            </li>
            <li>
              <a href="#">Ratings</a>
            </li>
            <li>
              <a href="#">Shop Help</a>
            </li>
            <li>
              <a href="#">Contacts us</a>
            </li>
          </ul>
        </div>
        <div>
          <h3>Sites</h3>
          <ul>
            <li><a href="#">DC</a></li>
            <li><a href="#">MAD Magazione</a></li>
            <li><a href="#">DS Kids</a></li>
            <li><a href="#">DS Universe</a></li>
            <li><a href="#">DS Power Visa</a></li>
          </ul>
        </div>
      </nav>

      <img src="../assets/img/dc-logo-bg.png" alt="" />
    </div>
  </section>
</template>

<script>
export default {
  name: "FooterMid",
};
</script>

<style scoped lang="scss">
@import "../assets/style/partials/variables.scss";

section {
  overflow-y: hidden;
  background: url("../assets/img/footer-bg.jpg");
  background-size: cover;

  img {
    margin: -70px 0;
  }

  nav {
    display: flex;
    gap: 50px;

    h3 {
      font-size: 1.5rem;
      text-transform: uppercase;
      margin-bottom: 20px;
    }

    ul {
      list-style: none;
      margin-bottom: 20px;

      li {
        margin: 5px 0;
        a {
          font-size: 0.8rem;
          color: #959595;
          text-decoration: none;

          &:hover {
            text-decoration: underline;
          }
        }
      }
    }
  }
}
</style>
