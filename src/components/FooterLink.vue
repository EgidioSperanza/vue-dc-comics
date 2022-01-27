<template>
  <div class="footer-link">
    <div class="footer-link-inner">
      <div class="link-box">
        <div class="col">
          <h3>DC Comics</h3>
          <ul>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>TV</li>
            <li>Games</li>
            <li>Videos</li>
            <li>News</li>
          </ul>

          <h3>Shop</h3>
          <ul>
            <li>Shop DC</li>
            <li>Shop DC Collectibles</li>
          </ul>
        </div>
        <div class="col">
          <h3>DC</h3>
          <ul>
            <li>Terms Of Use</li>
            <li>Privacy Policy (New)</li>
            <li>Ad Choises</li>
            <li>Advertising</li>
            <li>Jobs</li>
            <li>Subscriptions</li>
            <li>Talent Workshops</li>
            <li>CPSC Certificates</li>
            <li>Ratings</li>
            <li>Shop Help</li>
            <li>Contact Us</li>
          </ul>
        </div>
        <div class="col">
          <h3>Sites</h3>
          <ul>
              <li>DC</li>
              <li>MAD Magazine</li>
              <li>DC Kids</li>
              <li>DC Universe</li>
              <li>DC Power Visa</li>
          </ul>
        </div>
      </div>
      <div class="footer-logo"></div>
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

.footer-link {
  height: 400px;
  background: url("../assets/footer-bg.jpg");
  background-size: cover;

  .footer-link-inner {
    width: $inner-container-width;
    height: 100%;
    margin: 0 auto;
    display: flex;

    .link-box {
      width: 50%;
      padding: 20px 50px 20px 0;
      display: flex;
      justify-content: space-between;

      h3 {
        text-transform: uppercase;
        color: #fff;
        margin: 20px 0;
      }

      li {
        color: $footer-link-color;
        margin-bottom: 5px;
        cursor: pointer;
      }
    }
    .footer-logo {
      width: 50%;
      height: 100%;
      background: url("../assets/dc-logo-bg.png") no-repeat;
      background-position: center;
    }
  }
}
</style>