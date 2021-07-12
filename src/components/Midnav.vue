<template>
  <div class="midnav-full">
    <div class="container">
      <ul>
        <li>
          <span class="midnav-img"
            ><img
              src="../assets/buy-comics-digital-comics.png"
              alt="Buy Digital Comics"
          /></span>
          <span class="midnav-txt">DIGITAL COMICS</span>
        </li>
        <li>
          <span class="midnav-img"
            ><img
              src="../assets/buy-comics-merchandise.png"
              alt="Buy Merchandise" /></span
          ><span class="midnav-txt">DC MERCHANDISE</span>
        </li>
        <li>
          <span class="midnav-img"
            ><img
              src="../assets/buy-comics-subscriptions.png"
              alt="Subscriptions" /></span
          ><span class="midnav-txt">SUBSCRIPTION</span>
        </li>
        <li>
          <span class="midnav-img"
            ><img
              src="../assets/buy-comics-shop-locator.png"
              alt="Comic Shop Locator" /></span
          ><span class="midnav-txt">COMIC SHOP LOCATOR</span>
        </li>
        <li>
          <span class="midnav-img"
            ><img
              src="../assets/buy-dc-power-visa.svg"
              alt="Power Visa" /></span
          ><span class="midnav-txt">DC POWEER VISA</span>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "Midnav",
};
</script>

<style lang="scss" scoped>
// @import "../style/colors.scss";
.midnav-full {
  background-color: rgba(2, 130, 249, 255);
  .container {
    display: flex;
    align-items: center;
    justify-content: space-around;
    height: 100px;

    ul {
      display: flex;
      justify-content: space-around;
      li {
        color: white;
        list-style: none;
        padding: 0 20px;
        display: flex;
        align-items: center;
        font-size: 10px;
        .midnav-img {
          img {
            width: 30px;
            padding-right: 5px;
          }
        }
      }
    }
  }
}
</style>