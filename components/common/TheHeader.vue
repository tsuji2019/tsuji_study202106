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
  mounted: function () {
    //★スクロールしたらヘッダーの高さを変化させる
    let headerH = $("#header").outerHeight(true);
    console.log(headerH);

    function FixedAnime() {
      let scroll = $(window).scrollTop();
      //スクロールがヘッダーの高さを超えたらクラスを付与、そうでばければ除去
      if (scroll >= headerH) {
        $("#header").addClass("HeightMin");
      } else {
        $("#header").removeClass("HeightMin");
      }
    }
    //スクロールしたら実行
    $(window).scroll(function () {
      FixedAnime();
    });
  },
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
    padding: 2rem 9% 2rem 0;
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
          padding-right: 2.8rem;
          li {
            margin: 0 2.5rem;
            position: relative;
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
              cursor: pointer;
              overflow: hidden;
              &__text {
                position: absolute;
                left: 0;
                display: block;
                color: #fff;
                font-size: 17px;
                font-weight: bold;
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
              transition: all 0.15s;
            }
            .nav__item:hover .nav__item__text:nth-child(2) {
              top: 0;
              transition: all 0.15s;
            }
            // hover時の上のライン
            &::after {
              content: "";
              position: absolute;
              top: -5.1rem;
              left: -0.4rem;
              width: 100%;
              height: 0.4rem;
              background: #fff100;
              transition: transform .3s cubic-bezier(0.8, 0, 0.2, 1) 0s;
              transform: scale(0, 1);
              transform-origin: right top;
            }
            &:hover::after {
              transform: scale(1, 1);
              transform-origin: left top;
            }
          }
          li:nth-child(1) {
            width: 4.8rem;
            > a {
              width: 4.8rem;
            }
          }
          li:nth-child(2) {
            width: 5.1rem;
            > a {
              width: 5.1rem;
            }
          }
          li:nth-child(3) {
            width: 6.9rem;
            > a {
              width: 6.9rem;
            }
          }
          li:nth-child(4) {
            width: 5.5rem;
            > a {
              width: 5.5rem;
            }
          }
          li:nth-child(5) {
            width: 5.6rem;
            > a {
              width: 5.6rem;
            }
          }
          li:nth-child(6) {
            width: 6.5rem;
            > a {
              width: 6.5rem;
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
/*スクロールしたらヘッダーの高さを変化させる*/
#header.HeightMin {
  // animation: DownAnime 0.5s forwards;
  background: rgba(255, 255, 255, 0.95);
  transition: 0.3s;
  .header-inner {
    position: relative;
    width: 91%;
    height: 5rem;
    z-index: 999;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1.3rem 9% 1.3rem 0;
    color: #000;
    #g-nav {
      &-list {
        .nav {
          padding-right: 0;
          > li {
            margin: 0 1.8rem;
            .nav__item {
              width: 5rem;
              &__text {
                color: $color-black;
                font-size: 1.4rem;
              }
            }
            &::after {
              top: -2.8rem;
            }
          }
        }
      }
    }
    &:after {
      top: 3.8rem;
      right: 11rem;
      background: $color-black;
    }
    .openbtn {
      > span {
        background: $color-black;
        width: 2.4rem;
      }
    }
    .openbtn span:nth-of-type(2) {
      top: 0;
    }
    .openbtn.active span:nth-of-type(1) {
      background-color: #fff;
    }

    .openbtn.active span:nth-of-type(3) {
      background-color: #fff;
    }
  }
}

// .header {
//   height: 70px;
//   width: 100%;
//   z-index: 999;
//   display: flex;
//   justify-content: space-between;
//   align-items: center;
//   text-align: center;
//   padding: 2rem 12% 2rem 0;
// }
</style>
