<template>
  <header>
    <div class="header-inner">
      <div class="header-logo">
        <img src="@/assets/dc-logo.png" alt="DC Logo" />
      </div>
      <nav>
        <ul>
          <li>characters</li>
          <li class="active">comics</li>
          <li>movies</li>
          <li>tv</li>
          <li>games</li>
          <li>collectibles</li>
          <li>videos</li>
          <li>fans</li>
          <li>news</li>
          <li>shop</li>
        </ul>
      </nav>
    </div>
    <div class="jumbotron"></div>
  </header>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
header {
  .header-inner {
    width: 1200px;
    margin: 0 auto;
    height: 100px;
    display: flex;
    align-items: center;

    .header-logo {
      width: 40%;
      height: 100%;
      display: flex;
      align-items: center;
      img {
        max-height: 80%;
      }
    }

    nav {
      width: 60%;
      height: 100%;
      ul {
        height: 100%;
        list-style: none;
        text-transform: uppercase;
        display: flex;
        justify-content: space-between;
        li {
          height: 100%;
          cursor: pointer;
          display: flex;
          align-items: center;
          &:hover {
            color: #0282f9;
          }
          &.active {
            position: relative;
          }
          &.active::before {
            content: "";
            position: absolute;
            left: 10%;
            right: 10%;
            bottom: 0px;
            height: 6px;
            background-color: #0282f9;
          }
        }
      }
    }
  }
  .jumbotron{
      height: 500px;
      background: url('../assets/jumbotron.jpg');
      background-position: top center;
  }
}
</style>