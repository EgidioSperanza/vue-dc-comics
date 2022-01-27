<template>
  <nav>
    <ul>
      <li>characters</li>
      <li class="active">comics</li>
      <!-- TODO:active class assigned to the click -->
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
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/style/variables.scss";
nav {
  width: 60%;
  height: 100%;
  ul {
    height: 100%;
    text-transform: uppercase;
    display: flex;
    justify-content: space-between;
    li {
      height: 100%;
      cursor: pointer;
      display: flex;
      align-items: center;
      &:hover {
        color: $primary-link-color;
      }
      &.active {
        position: relative;
        &::before {
          content: "";
          position: absolute;
          left: 10%;
          right: 10%;
          bottom: 0px;
          height: 6px;
          background-color: $primary-link-color;
        }
      }
    }
  }
}
</style>