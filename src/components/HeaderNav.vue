<template>
  <nav>
    <ul>
      <li v-for="link in navLinks" :key="link.id">
        {{ link.nameLink }}
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  props: {
    navLinks: Array,
  },
};
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
        position: relative;
        color: $primary-link-color;
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