<template>
  <div class="header-full">
    <div class="container">
      <div class="header-logo">
        <img src="../assets/dc-logo.png" alt="Dc comics logo" />
      </div>
      <nav>
        <ul>
          <li><a href="">CHARACTERS</a></li>
          <li><a href="">COMICS</a></li>
          <li><a href="">MOVIES</a></li>
          <li><a href="">TV</a></li>
          <li><a href="">GAMES</a></li>
          <li><a href="">COLLECTIBILES</a></li>
          <li><a href="">VIDEOS</a></li>
          <li><a href="">FANS</a></li>
          <li><a href="">NEWS</a></li>
          <li><a href="">SHOP</a></li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
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