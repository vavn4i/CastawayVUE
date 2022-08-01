<template>
  <footer class="footer container">
    <div class="footer__logo">
      <a href="#"><img src="../images/logo.png" alt="" class="logo" /></a>
      <ul class="social">
        <li class="social__item">
          <a href="#">
            <img src="../images/inst.svg" alt="" />
          </a>
        </li>
        <li class="social__item">
          <a href="#">
            <img src="../images/twitter.svg" alt="" />
          </a>
        </li>
        <li class="social__item">
          <a href="#">
            <img src="../images/facebook.svg" alt="" />
          </a>
        </li>
      </ul>
    </div>
    <ul class="pages">
      <li class="page">
        <a href="#">Home</a>
      </li>
      <li class="page">
        <a href="#">About</a>
      </li>
      <li class="page">
        <a href="#">Episodes</a>
      </li>
      <li class="page">
        <a href="#">Contact</a>
      </li>
    </ul>
    <ul class="sections">
      <li class="section">
        <a href="#">Style Guide</a>
      </li>
      <li class="section">
        <a href="#">Instructions</a>
      </li>
      <li class="section">
        <a href="#">Changelog</a>
      </li>
      <li class="section">
        <a href="#">Credit</a>
      </li>
      <li class="section">
        <a href="#">Powered by Webflow</a>
      </li>
      <li class="section">
        <a href="#">Licenses</a>
      </li>
    </ul>
    <ul class="platforms">
      <li class="platform">
        <a href="#">
          <img src="../images/spotify.svg" alt="" />
        </a>
      </li>
      <li class="platform">
        <a href="#">
          <img src="../images/spotufyRed.svg" alt="" />
        </a>
      </li>
      <li class="platform">
        <a href="#">
          <img src="../images/sky.svg" alt="" />
        </a>
      </li>
      <li class="platform">
        <a href="#">
          <img src="../images/podcasts.svg" alt="" />
        </a>
      </li>
      <li class="platform">
        <a href="#">
          <img src="../images/radio.svg" alt="" />
        </a>
      </li>
    </ul>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  components: {},
};
</script>

<style lang="scss">
.footer {
  padding-bottom: 127px;
  display: flex;
  &__logo {
    margin-right: 240px;
    .logo {
      margin-bottom: 20px;
      width: 224px;
      height: 46px;
    }
    .social {
      display: flex;
      &__item {
        margin-right: 10px;
        cursor: pointer;
        &:last-child {
          margin-right: 0;
        }
      }
    }
  }

  .pages {
    margin-right: 120px;
    .page {
      margin-bottom: 10px;
      &:last-child {
        margin-bottom: 0;
      }

      a {
        font-size: 17px;
        color: #ffffff;
        cursor: pointer;
        &:hover {
          color: #118da8;
        }
      }
    }
  }

  .sections {
    margin-right: 20px;
    .section {
      margin-bottom: 10px;
      &:last-child {
        margin-bottom: 0;
      }

      a {
        font-size: 17px;
        color: #ffffff;
        cursor: pointer;
        &:hover {
          color: #118da8;
        }
      }
    }
  }

  .platforms {
    display: flex;

    .platform {
      margin-right: 17px;
      &:last-child {
        margin-right: 0;
      }

      a {
        cursor: pointer;
        &:hover {
          color: #118da8;
        }
      }
    }
  }
}
</style>
