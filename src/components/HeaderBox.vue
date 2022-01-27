<template>
  <header>
    <div class="header-inner">
        <header-logo />
        <header-nav />
    </div>
    <div class="jumbotron"></div>
  </header>
</template>

<script>
import HeaderLogo from '@/components/HeaderLogo.vue'
import HeaderNav from '@/components/HeaderNav.vue';

export default {
  components: { 
      HeaderLogo,
      HeaderNav
   },
};
</script>

<style lang="scss" scoped>
@import "@/style/variables.scss";

header {
  .header-inner {
    width: $inner-container-width;
    margin: 0 auto;
    height: 100px;
    display: flex;
    align-items: center;

  }
  .jumbotron{
      height: 500px;
      background: url('../assets/jumbotron.jpg') no-repeat;
      background-position: top center;
      background-size:cover ;
  }
}
</style>