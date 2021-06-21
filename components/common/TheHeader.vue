<template>
  <header id="header">
    <div class="header-inner">
      <h1 class="logo">
        <a href=""><LogoSvg /></a>
      </h1>
      <nav id="g-nav">
        <div id="g-nav-list">
          <ul id="g-navi" class="nav">
            <li>
              <a href="#" class="nav__item">
                <span class="nav__item__text">About</span>
                <span class="nav__item__text">About</span>
              </a>
            </li>
            <li>
              <a href="#" class="nav__item">
                <span class="nav__item__text">Works</span>
                <span class="nav__item__text">Works</span>
              </a>
            </li>
            <li>
              <a href="#" class="nav__item">
                <span class="nav__item__text">Findings</span>
                <span class="nav__item__text">Findings</span>
              </a>
            </li>
            <li>
              <a href="#" class="nav__item">
                <span class="nav__item__text">Events</span>
                <span class="nav__item__text">Events</span>
              </a>
            </li>
            <li>
              <a href="#" class="nav__item">
                <span class="nav__item__text">People</span>
                <span class="nav__item__text">People</span>
              </a>
            </li>
            <li>
              <a href="#" class="nav__item">
                <span class="nav__item__text">Contact</span>
                <span class="nav__item__text">Contact</span>
              </a>
            </li>
          </ul>
        </div>
        <div></div>
      </nav>
      <!-- ハンバーガーメニュー -->
      <!-- アイコン -->
      <div class="openbtn">
        <span></span>
        <span></span>
        <span></span>
      </div>
      <!-- メニューインナー -->
      <nav id="g-nav2">
        <div id="g-nav2-list">
          <ul>
            <li class="blurTrigger blur"><a href="#"></a></li>
            <li class="blurTrigger blur"><a href="#"></a></li>
            <li class="blurTrigger blur"><a href="#"></a></li>
            <li class="blurTrigger blur"><a href="#"></a></li>
            <li class="blurTrigger blur"><a href="#"></a></li>
          </ul>
        </div>
      </nav>
    </div>
  </header>
</template>

<script>
import LogoSvg from "~/assets/svg/Logo.svg?inline";

export default {
  components: {
    LogoSvg,
  },
  //   mounted: function () {
  //   },
};
</script>

<style lang="scss" scoped>
@import "~assets/scss/variables";

#header {
  width: 100%;
  position: fixed;
  font-family: $font-header;
  font-weight: bold;
  z-index: 100;
  .header-inner {
    position: relative;
    width: 91%;
    height: 8.2rem;
    z-index: 999;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 9% 20px 0;
    .logo {
      text-transform: uppercase;
      padding: 0 0 0 2%;
      line-height: 1;
      white-space: nowrap;
    }
    #g-nav {
      &-list {
        .nav {
          display: flex;
          justify-content: center;
          // color: #000000;
          // padding-right: 3rem;
          overflow: hidden;
          li {
            height: 2.2rem;
            > a {
              color: #fff;
              padding: 1rem 2rem;
              letter-spacing: 0.05rem;
              transition: all 0.3s;
              font-weight: 900;
              font-size: 1.6rem;
            }
            /* ボタン本体 */
            .nav__item {
              position: relative;
              display: inline-block;
              width: 6.8rem;
              // height: 1.2rem;
              // overflow: hidden;
              cursor: pointer;
              &__text {
                position: absolute;
                left: 0;
                display: block;
                // height: 1.2rem;
                width: 6.8rem;
                color: #fff; /* 文字色 */
                font-size: 16px; /* 文字サイズ */
                font-weight: bold; /* 文字の太さ */
                text-align: center; /* テキストを中央揃え */
                transition: all 0.15s;
                padding-top: 1rem;
              }
              &__text:nth-child(1) {
                top: 0;
              }
              &__text:nth-child(2) {
                top: -100%;
              }
            }
            /* ボタンホバーアクション */
            .nav__item:hover .nav__item__text:nth-child(1) {
              top: 100%;
            }

            .nav__item:hover .nav__item__text:nth-child(2) {
              top: 0;
            }
          }
        }
      }
    }
    &:after {
      position: absolute;
      top: 61px;
      bottom: 0;
      right: 12rem;
      display: block;
      content: "";
      width: 1px;
      height: 20px;
      margin-top: -10px;
      background: #fff;
    }
  }
}
.header {
  height: 70px;
  width: 100%;
  z-index: 999;
  display: flex;
  justify-content: space-between;
  align-items: center;
  text-align: center;
  padding: 2rem 12% 2rem 0;
}
</style>
