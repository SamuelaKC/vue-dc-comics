<template>
  <div class="container">
    <div class="content-1">
      <div class="footer-main-1">
        <div class="menu">
          <div class="text-title">DC COMICS</div>
          <div><a href="#">Characters</a></div>
          <div><a href="#">Comics</a></div>
          <div><a href="#">TV</a></div>
          <div><a href="#">Games</a></div>
          <div><a href="#">Videos</a></div>
          <div><a href="#">News</a></div>
        </div>

        <div class="menu">
          <div class="text-title">SHOP</div>
          <div><a href="#">Shop DC</a></div>
          <div><a href="#">Shop DC Collectibles</a></div>
        </div>
      </div>
      <div class="footer-main-2">
        <div class="menu">
          <div class="text-title">DC</div>
          <div><a href="#">Terms Of Use</a></div>
          <div><a href="#">Privacy podivcy (New)</a></div>
          <div><a href="#">Ad Choices</a></div>
          <div><a href="#">Advertising</a></div>
          <div><a href="#">Jobs</a></div>
          <div><a href="#">Subscriptions</a></div>
          <div><a href="#">Talent Workshops</a></div>
          <div><a href="#">CPSC Certificates</a></div>
          <div><a href="#">Raiting</a></div>
          <div><a href="#">Shop Help</a></div>
          <div><a href="#">Contact Us</a></div>
        </div>
      </div>

      <div class="footer-main-3">
        <div class="menu">
          <div class="text-title">SITES</div>
          <div><a href="#">DC</a></div>
          <div><a href="#">MAD Magazine</a></div>
          <div><a href="#">DC Kids</a></div>
          <div><a href="#">DC Universe</a></div>
          <div><a href="#">DC Power Visa</a></div>
        </div>
      </div>

      <div class="footer-image">
        <img src="../assets/dc-logo-bg.png" alt="" />
      </div>
    </div>
    <div class="content-2">
      <div class="footer-second-1">
        <div class="button">SIGN-UP NOW!</div>
      </div>
      <div class="footer-second-2">
        <div class="follow">
          <div class="follow-text">FOLLOW US</div>
          <div class="follow-image">
            <img src="../assets/footer-facebook.png" alt="facebook" />
            <img src="../assets/footer-twitter.png" alt="twitter" />
            <img src="../assets/footer-youtube.png" alt="youtube" />
            <img src="../assets/footer-pinterest.png" alt="pinterest" />
            <img src="../assets/footer-periscope.png" alt="periscope" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Footer',
}
</script>

<style lang="scss" scoped>
@import '../style/colors.scss';
@import '../style/fonts.scss';

.content-1 {
  background-image: url(../assets/footer-bg.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  height: 400px;
  display: flex;
  justify-content: space-around;

  [class^='footer-main-'] {
    flex-grow: 2;
    margin-top: 20px;

    &:first-child {
      margin-left: 300px;
    }
  }

  .footer-image {
    text-align: right;
    position: relative;
    z-index: 20;
    flex-grow: 1;
    margin-right: 100px;
    width: 350px;
    img {
      width: 100%;
    }
  }

  .text-title {
    color: $bg-font-color;
    font-size: 20px;
    font-weight: 700;
  }

  .menu {
    width: 50%;
    list-style: none;
    font-size: 12px;
    margin: 5px 0;

    a {
      color: $footer-link-color;
      text-decoration: none;
    }
  }
}

.content-2 {
  display: flex;
  justify-content: space-around;
  position: relative;
  z-index: 30;
  height: 80px;
  background-color: $bg-color-footer;

  .button {
    width: 150px;
    padding: 10px;
    border: 2px solid $bg-color-blue;
    color: $bg-font-color;
    text-align: center;
    font-weight: 700;
  }

  .follow {
    display: flex;
    align-items: center;
  }

  .follow-text {
    color: $bg-color-blue;
    font-size: 20px;
    font-weight: 700;
  }

  .follow-image {
    img {
      margin-left: 20px;
    }
  }

  [class^='footer-second-'] {
    flex-grow: 2;
    margin-top: 20px;

    &:first-child {
      margin-left: 300px;
    }
  }
}
</style>
