<template>
  <main>
    <div class="main-inner">--Contents goes here--</div>
  </main>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/style/variables.scss";

main {
  height: 100px;
  line-height: 100px;
  font-size: 20px;
  color: white;
  background-color: #333;

  .main-inner {
    width: $inner-container-width;
    margin: 0 auto;
  }
}
</style>