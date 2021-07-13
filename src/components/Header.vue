<template>
  <div class="header-full">
    <div class="container">
      <div class="header-logo">
        <img src="../assets/dc-logo.png" alt="Dc comics logo" />
      </div>
      <nav>
        <ul>
          <li v-for="item in navBar" :key="item.navItem"><a href="">{{item.navItem}}</a></li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
  props: {
    navItem: String,
    id: Number,
  },
  data() {
    return {
      navBar: [
        {navItem: "CHARACTERS", id: 0},
        {navItem: "COMICS", id: 1},
        {navItem: "MOVIES", id: 2},
        {navItem: "TV", id: 3},
        {navItem: "GAMES", id: 4},
        {navItem: "COLLECTIBILES", id: 5},
        {navItem: "VIDEOS", id: 6},
        {navItem: "FANS", id: 7},
        {navItem: "NEWS", id: 8},
        {navItem: "SHOP", id: 9},
      ]
    }
  }
};
</script>

<style lang="scss" scoped>
// @import "../style/colors.scss";
.header-full {
  height: 80px;
  .container {
    display: flex;
    justify-content: space-between;

    .header-logo {
      display: flex;
      align-items: center;
      height: 80px;

      img {
        width: 50px;
      }
    }

    ul {
      display: flex;
      align-items: center;
      height: 80px;

      li {
        list-style: none;
        display: flex;
        align-items: center;
        height: 100%;

        &:hover {
          border-bottom: 2px solid #0282f9;
        }
        a {
          text-decoration: none;
          font-size: 10px;
          padding: 0 5px;
          color: black;

          &:hover {
            color: #0282f9;
          }
        }
      }
    }
  }
}
</style>