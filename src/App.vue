<template>
  <div id="app">
    <header-box />
    <main-container />
    <footer-box />
  </div>
</template>

<script>
import HeaderBox from './components/HeaderBox.vue'
import MainContainer from './components/MainContainer.vue'
import FooterBox from './components/FooterBox.vue'

export default {
  name: 'App',
  components: {
    HeaderBox,
    MainContainer,
    FooterBox
  }
}
</script>

<style lang="scss">
@import './style/main.scss'
</style>
