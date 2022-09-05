<template>
  <section>
    <div class="container">
      <a href="#" class="signup">Sign-up now!</a>

      <div class="social">
        <h3>Follow us</h3>

        <ul>
          <li>
            <a href="#"
              ><img src="../assets/img/footer-facebook.png" alt="Facebook"
            /></a>
          </li>
          <li>
            <a href="#"
              ><img src="../assets/img/footer-twitter.png" alt="Twitter"
            /></a>
          </li>
          <li>
            <a href="#"
              ><img src="../assets/img/footer-youtube.png" alt="YouTube"
            /></a>
          </li>
          <li>
            <a href="#"
              ><img src="../assets/img/footer-pinterest.png" alt="Pinterest"
            /></a>
          </li>
          <li>
            <a href="#"
              ><img src="../assets/img/footer-periscope.png" alt="Periscope"
            /></a>
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "FooterBot",
};
</script>

<style scoped lang="scss">
@import "../assets/style/partials/variables.scss";

section {
  padding: 50px 0;
  background: #303030;

  a.signup {
    border: 3px solid $accent;
    padding: 15px;
    font-size: 1.4rem;
    color: #fff;
    text-decoration: none;
    text-transform: uppercase;

    &:hover {
      background: $accent;
    }
  }

  .social {
    display: flex;
    gap: 30px;

    h3 {
      font-size: 1.6rem;
      color: $accent;
      text-transform: uppercase;
    }

    ul {
      list-style: none;

      li {
        display: inline;
        margin: 10px;
      }
    }
  }
}
</style>
