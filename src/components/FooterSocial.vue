<template>
  <div class="footer-social">
    <div class="footer-social-inner">
      <div class="footer-signin">
        <a href="#">SIGN-UP NOW!</a>
      </div>
      <div class="footer-social-link">
          <h3>Follow us</h3>
          <ul>
              <li><img src="@/assets/footer-facebook.png" alt="Facebook"></li>
              <li><img src="@/assets/footer-twitter.png" alt="Twitter"></li>
              <li><img src="@/assets/footer-youtube.png" alt="YouTube"></li>
              <li><img src="@/assets/footer-pinterest.png" alt="Pinterest"></li>
              <li><img src="@/assets/footer-periscope.png" alt="Location"></li>
          </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
};
</script>

<style lang="scss" scoped>
@import "@/style/variables.scss";

.footer-social {
  background-color: $footer-social-bkg;

  .footer-social-inner {
    width: $inner-container-width;
    margin: 0 auto;
    padding: 40px 0;
    display: flex;
    justify-content: space-between;

    .footer-signin{
        width: 60%;
        display: flex;
        align-items: center;
        a{
            padding: 10px;
            border: 3px solid $primary-link-color;
            text-decoration: none;
            color: #FFF;
        }
    }

    .footer-social-link{
        width: 40%;
        display: flex;
        align-items: center;
        justify-content: space-between;
        h3{
            text-transform: uppercase;
            color: $primary-link-color;
        }
        ul{
            width: 70%;
            display: flex;
            justify-content: space-between;
        }

    }
  }
}
</style>