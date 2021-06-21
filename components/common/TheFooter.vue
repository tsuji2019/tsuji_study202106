<template>
  <footer class="footer">
      <a href="#" class="f-btn01 btn bgleft"><p class="btn-text">
        <span class="btn-title">オンライン相談</span><br>
          プロジェクトのご相談を随時受付中！<br />
          「ロフトワークにこんなこと頼めますか？」「まだプロジェクト化していないのだけど、早めに相談したい」<br />
          など、まずはお気軽にお声掛けください。オンライン相談はその場で日時予約が可能です。</p></a>
    <div class="f-btn02">
      <ul>
        <li>
          <a href="" class="btn-ft bgleft">
            <div class="btn-inner btn-text">
              <p class="btn-icon"><CalenderSvg /></p>
              <p class="btn-title">開催予定のイベント</p>
              <span class="btn-text">
                テーマは「経営」から「子ども向け工作」まで、<br />
                毎日さまざまな種類のイベントを開催しています。
              </span>
            </div>
          </a>
        </li>
        <li>
          <a href="" class="btn-ft bgleft">
            <div class="btn-inner btn-text">
              <p class="btn-icon"><BuildingSvg /></p>
              <p class="btn-title">開催予定のイベント</p>
              <span class="btn-text">
                テーマは「経営」から「子ども向け工作」まで、<br />
                毎日さまざまな種類のイベントを開催しています。
              </span>
            </div>
          </a>
        </li>
        <li>
          <a href="" class="btn-ft bgleft">
            <div class="btn-inner btn-text">
              <p class="btn-icon"><MailmagazineSvg /></p>
              <p class="btn-title">開催予定のイベント</p>
              <span class="btn-text">
                テーマは「経営」から「子ども向け工作」まで、<br />
                毎日さまざまな種類のイベントを開催しています。
              </span>
            </div>
          </a>
        </li>
      </ul>
    </div>
    <div class="ft-nav">
      <div class="ft-nav__box">
        <dl>
          <dt>Who We Are</dt>
          <dd><a href="#">People</a></dd>
        </dl>
        <dl>
          <dt>What We Do</dt>
          <dd><a href="#">UX</a></dd>
          <dd><a href="#">新規事業</a></dd>
          <dd><a href="#">サービスデザイン</a></dd>
          <dd><a href="#">デザインリサーチ</a></dd>
          <dd><a href="#">大学</a></dd>
          <dd><a href="#">グローバル</a></dd>
          <dd><a href="#">Web</a></dd>
        </dl>
        <dl>
          <dt>How We Work</dt>
          <dd><a href="#">Pプロジェクトの実践で得た知見</a></dd>
          <dd><a href="#">わたしたちの手法・思考</a></dd>
        </dl>
        <dl>
          <dt>Where We Are</dt>
          <dd><a href="#">Tokyo</a></dd>
          <dd><a href="#">TKyoto</a></dd>
          <dd><a href="#">Hida</a></dd>
          <dd><a href="#">Taiwan</a></dd>
          <dd><a href="#">Hong Kong</a></dd>
          <dd><a href="#">FabCafe Global</a></dd>
        </dl>
        <dl>
          <dt>Information</dt>
          <dd><a href="#">Company Profile</a></dd>
          <dd><a href="#">News&Column</a></dd>
          <dd><a href="#">Event</a></dd>
        </dl>
        <dl>
          <dt>Platforms</dt>
          <dd><a href="#">FabCafe</a></dd>
          <dd><a href="#">MTRL</a></dd>
          <dd><a href="#">Hidakuma</a></dd>
          <dd><a href="#">OpenCu</a></dd>
          <dd><a href="#">AWRD</a></dd>
          <dd><a href="#">Layout</a></dd>
        </dl>
        <dl>
          <dt>SNS</dt>
          <dd><a href="#">Twitter</a></dd>
          <dd><a href="#">Facebook</a></dd>
          <dd><a href="#">Instagram</a></dd>
        </dl>
        <dl>
          <dd><a href="#">Recruit</a></dd>
          <dd><a href="#">Contact</a></dd>
          <dd><a href="#">Privacy Policy</a></dd>
          <dd><a href="#">Terms of Use</a></dd>
        </dl>
      </div>
    </div>
    <div class="copylight">
      <p>©2021 Loftwork Inc. All rights reserved</p>
    </div>
  </footer>
</template>

<script>
import LogoSvg from "~/assets/svg/Logo.svg?inline";
import CalenderSvg from "~/assets/svg/calender.svg?inline";
import BuildingSvg from "~/assets/svg/building.svg?inline";
import MailmagazineSvg from "~/assets/svg/mailmagazine.svg?inline";

export default {
  components: {
    LogoSvg,
    CalenderSvg,
    BuildingSvg,
    MailmagazineSvg,
  },
};
</script>

<style lang="scss" scoped>
@import "~assets/scss/variables";

footer {
  width: 100%;
  .f-btn01 {
    text-align: center;
    background-color: #e6da00;
    padding: 8rem 0;
    width: 100%;
    // height: 29.4rem;
    &:hover {
      background-color: #fff880;
    }
    // .f-eff01 {
    //   width: 100%;
    //   height: 29.4rem;
    // }
    > a {
      color: $color-black;
      > p {
        > span {
        }
      }
    }
  }
  .f-btn02 {
    position: relative;
    margin: 0 auto;
    width: 100%;
    > ul {
      display: flex;
      justify-content: space-between;
      > li {
        text-align: center;
        width: -webkit-calc(100% / 3);
        width: calc(100% / 3);
        position: relative;
        > a {
          color: $color-white;
          > .btn-inner {
            padding: 16rem 0;
            display: inline-block;
          }
        }
        &:nth-child(2) {
          background: #262a42;
        }
        &:nth-child(3) {
          background: #22263d;
        }
      }
    }
  }
  .ft-nav {
    background-color: #1f2336;
    padding: 7rem 15rem;
    &__box {
      color: $color-white;
      display: flex;
      justify-content: space-between;
      flex-wrap: wrap;
      > dl {
        width: -webkit-calc(100% / 4);
        width: calc(100% / 4);
        display: block;
        padding: 5rem 0;
        letter-spacing: 0.05rem;
        > dt {
          font-size: 1.9rem;
          font-weight: 700;
          margin-bottom: 3rem;
        }
        > dd {
          font-size: 1.1rem;
          font-weight: 300;
          margin-bottom: 1.8rem;
          > a {
            font-weight: 300;
            &:hover {
              text-decoration: underline;
              opacity: 1;
            }
          }
        }
      }
    }
  }
  .copylight {
    width: 100%;
    background-color: #12141d;
    > p {
      color: $color-white;
      font-size: 1rem;
      font-weight: 700;
      padding: 25rem 12rem 10rem;
      text-align: right;
    }
  }
  .btn-inner {
    padding: 8rem 0;
  }
  .btn-title {
    font-size: 2.3rem;
    padding: 0 0 2.2rem;
    display: inline-block;
    font-weight: 900;
    z-index: 2;
    // font-family: $font-midash;
  }
  .btn-text {
    font-size: 1.2rem;
    position: relative;
    display: block;
    font-weight: 300;
    line-height: 2;
    letter-spacing: 0.01rem;
    z-index: 2;
  }
  .btn-icon {
    margin-bottom: 1rem;
  }
  // ボタン/hoverアニメーション
  .btn-ft {
  position: relative;
  overflow: hidden;
  display: inline-block;
  text-align: center;
  background: #2e334f;
  width: 100%;
  height: 100%;
}
.btn-ft span {
  position: relative;
  z-index: 3;
}
  .btn-animation {
    cursor: pointer;
    position: relative;
    box-sizing: border-box;
    overflow: hidden;
    a {
      transition: 1s;
      z-index: 2;
      position: relative;
    }
  svg {
    fill: currentColor;
  }
}
  svg {
    fill: currentColor;
  }
}
</style>
