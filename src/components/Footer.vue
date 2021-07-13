<template>
  <div class="container">
    <div class="content-1">
      <MainSectionBlue />
    </div>
    <div class="content-2">
      <div class="footer-main-1">
        <div class="menu-1">
          <div class="text-title">DC COMICS</div>
          <div><a href="#">Characters</a></div>
          <div><a href="#">Comics</a></div>
          <div><a href="#">TV</a></div>
          <div><a href="#">Games</a></div>
          <div><a href="#">Videos</a></div>
          <div><a href="#">News</a></div>
        </div>

        <div class="menu-2">
          <div class="text-title">SHOP</div>
          <div><a href="#">Shop DC</a></div>
          <div><a href="#">Shop DC Collectibles</a></div>
        </div>
      </div>
      <div class="footer-main-2">
        <div class="menu-1">
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
        <div class="menu-1">
          <div class="text-title">SITES</div>
          <div><a href="#">DC</a></div>
          <div><a href="#">MAD Magazine</a></div>
          <div><a href="#">DC Kids</a></div>
          <div><a href="#">DC Universe</a></div>
          <div><a href="#">DC Power Visa</a></div>
        </div>
      </div>

      <div class="footer-image">
        <img src="../assets/dc-logo-bg.png" alt="logo" />
      </div>
    </div>
    <div class="content-3">
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
import MainSectionBlue from '@/components/MainSectionBlue.vue'

export default {
  name: 'Footer',
  components: {
    MainSectionBlue,
  },
}
</script>

<style lang="scss" scoped>
@import '../style/colors.scss';
@import '../style/fonts.scss';

.content-1 {
  position: absolute;
  width: 100%;
  z-index: 1;
}

.content-2 {
  background-image: url(../assets/footer-bg.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  height: 500px;
  display: flex;
  justify-content: space-around;

  [class^='footer-main-'] {
    flex-grow: 2;
    margin-top: 70px;

    &:first-child {
      margin-left: 350px;
    }
  }

  .footer-image {
    flex-grow: 1;
    margin-right: 100px;
    width: 450px;
    img {
      width: 100%;
    }
  }

  .text-title {
    color: $bg-font-color;
    font-size: 20px;
    font-weight: 700;
  }

  [class^='menu-'] {
    list-style: none;
    font-size: 12px;

    div {
      padding-top: 10px;
    }

    a {
      color: $footer-link-color;
      text-decoration: none;
    }
  }

  .menu-1 {
    margin-top: 75px;
  }

  .menu-2 {
    margin-top: 25px;
  }
}

.content-3 {
  display: flex;
  justify-content: space-around;
  position: relative;
  z-index: 1;
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
