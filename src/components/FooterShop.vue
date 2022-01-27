<template>
  <div class="footer-shop">
    <ul>
      <li>
        <img
          src="@/assets/buy-comics-digital-comics.png"
          alt="Buy Digital Comics"
        />
        <span>Digital Comics</span>
      </li>
      <li>
        <img src="@/assets/buy-comics-merchandise.png" alt="Buy Merchandise" />
        <span>DC Merchandise</span>
      </li>
      <li>
        <img
          src="@/assets/buy-comics-subscriptions.png"
          alt="Buy Subscriptions"
        />
        <span>Subscription</span>
      </li>
      <li>
        <img
          src="@/assets/buy-comics-shop-locator.png"
          alt="Comic Shop Locator"
        />
        <span>comic shop locator</span>
      </li>
      <li>
        <img src="@/assets/buy-dc-power-visa.svg" alt="Power Visa" />
        <span>DC power visa</span>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  components: {},
};
</script>

<style lang="scss" scoped>
@import "@/style/variables.scss";

.footer-shop {
  background-color: $primary-link-color;
  padding: 50px 0;
  display: flex;
  justify-content: space-between;
  ul {
    width: $inner-container-width;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;

    li {
      cursor: pointer;
      display: flex;
      align-items: center;

      img {
        height: 60px;
      }

      span {
        text-transform: uppercase;
        color: $footer-ico-link-color;
        padding-left: 20px;
      }
    }
  }
}
</style>