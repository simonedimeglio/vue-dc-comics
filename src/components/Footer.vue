<template>
  <footer class="footer-full">
    <div class="container">
      <div class="footer-list-container">
        <div class="footer-column column-1">
          <ul>
            <li>DC COMICS</li>
            <li><a href="">Characters</a></li>
            <li><a href="">Comics</a></li>
            <li><a href="">Movies</a></li>
            <li><a href="">TV</a></li>
            <li><a href="">Games</a></li>
            <li><a href="">Videos</a></li>
            <li><a href="">News</a></li>
          </ul>
          <ul>
            <li>SHOP</li>
            <li><a href="">Shop DC</a></li>
            <li><a href="">Shop DC Collectibles</a></li>
          </ul>
        </div>
        <div class="footer-column column-2">
          <ul>
            <li>DC</li>
            <li><a href="">Terms Of Use</a></li>
            <li><a href="">Privacy policy (New)</a></li>
            <li><a href="">Ad Choices</a></li>
            <li><a href="">Advertising</a></li>
            <li><a href="">Jobs</a></li>
            <li><a href="">Subscriptions</a></li>
            <li><a href="">Talent Workshop</a></li>
            <li><a href="">CPSC Certificates</a></li>
            <li><a href="">Ratings</a></li>
            <li><a href="">Shop Help</a></li>
            <li><a href="">Contact Us</a></li>
          </ul>
        </div>
        <div class="footer-column column-3">
          <ul>
            <li>SITES</li>
            <li><a href="">DC</a></li>
            <li><a href="">MAD Magazine</a></li>
            <li><a href="">DC Kids</a></li>
            <li><a href="">DC Universe</a></li>
            <li><a href="">DC Power Visa</a></li>
            <li><a href="">Videos</a></li>
            <li><a href="">News</a></li>
          </ul>
        </div>
      </div>
      <div class="footer-dc-logo">
        <img src="../assets/dc-logo-bg.png" alt="Dc Logo" />
      </div>
    </div>
    <div class="sub-footer">
      <div class="container">
        <div class="sign-up-button">SIGN-UP NOW!</div>
        <div class="social">
          <ul>
            <li>FOLLOW US</li>
            <li>
              <a href=""
                ><img src="../assets/footer-facebook.png" alt="Facebook"
              /></a>
            </li>
            <li>
              <a href=""
                ><img src="../assets/footer-twitter.png" alt="Twitter"
              /></a>
            </li>
            <li>
              <a href=""
                ><img src="../assets/footer-youtube.png" alt="YouTube"
              /></a>
            </li>
            <li>
              <a href=""
                ><img src="../assets/footer-pinterest.png" alt="Pinterest"
              /></a>
            </li>
            <li>
              <a href=""
                ><img src="../assets/footer-periscope.png" alt="Periscope"
              /></a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style lang="scss" scoped>
// @import "../style/colors.scss";
.footer-full {
  background-image: url("../assets/footer-bg.jpg");
  .container {
    color: white;
    display: flex;
    justify-content: space-between;
    .footer-list-container {
      display: flex;
      padding-top: 20px;

      .footer-column {
        ul {
          margin-right: 15px;
          li {
            list-style: none;
            font-size: 10px;
            padding-top: 5px;

            &:first-child {
              font-weight: bold;
              font-size: 12px;
              padding: 10px 0 5px 0;
            }
          }
          a {
            text-decoration: none;
            color: gray;

            &:hover {
              color: white;
              cursor: pointer;
            }
          }
        }
      }
    }

    .footer-dc-logo {
      height: 250px;
      display: flex;
      align-items: center;
      overflow: hidden;
      img {
        height: 350px;
        width: 350px;
      }
    }
  }

  .sub-footer {
    padding: 20px 0;
    background-color: #303030;
    color: white;
    .container {
      display: flex;
      align-items: center;
      justify-content: space-between;
      .sign-up-button {
        border: 1px solid #0282f9;
        padding: 10px;
        font-size: 12px;
        font-weight: bold;

        &:hover {
          cursor: pointer;
          text-decoration: underline;
        }
      }
      .social {
        ul {
          display: flex;
          justify-content: center;
          align-items: center;
          list-style: none;
          li {
            padding: 0 5px;

            &:first-child {
              font-size: 12px;
              color: #0282f9;
              font-weight: bold;
            }
            a {
              img {
                width: 20px;
                &:hover {
                  cursor: pointer;
                }
              }
            }
          }
        }
      }
    }
  }
}
</style>