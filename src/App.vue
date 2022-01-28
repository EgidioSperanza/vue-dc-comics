<template>
  <div id="app">
    <header-box :navLinks="navLinks" />
    <main-container />
    <footer-box />
  </div>
</template>

<script>
import HeaderBox from "./components/HeaderBox.vue";
import MainContainer from "./components/MainContainer.vue";
import FooterBox from "./components/FooterBox.vue";

export default {
  name: "App",
  components: {
    HeaderBox,
    MainContainer,
    FooterBox,
  },
  data() {
    return {
      navLinks: [
        {
          id:"lnk001",
          nameLink:"characters",
          isActive:false,
        },
        {
          id:"lnk002",
          nameLink:"comics",
          isActive:false,
        },
        {
          id:"lnk003",
          nameLink:"movies",
          isActive:false,
        },
        {
          id:"lnk004",
          nameLink:"tv",
          isActive:false,
        },
        {
          id:"lnk005",
          nameLink:"games",
          isActive:false,
        },
        {
          id:"lnk006",
          nameLink:"collectibles",
          isActive:false,
        },
        {
          id:"lnk007",
          nameLink:"videos",
          isActive:false,
        },
        {
          id:"lnk008",
          nameLink:"fans",
          isActive:false,
        },
        {
          id:"lnk009",
          nameLink:"news",
          isActive:false,
        },
        {
          id:"lnk010",
          nameLink:"shop",
          isActive:false,
        },
      ]
    }
  },
};
</script>

<style lang="scss">
@import "./style/main.scss";
</style>
