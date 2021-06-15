<template>
  <footer class="footer">
    <div class="f-btn01">
      <a href="">
        <div class="btn-inner">
          <p class="btn-title">オンライン相談</p>
          <span class="btn-text"
            >プロジェクトのご相談を随時受付中！<br />
            「ロフトワークにこんなこと頼めますか？」「まだプロジェクト化していないのだけど、早めに相談したい」<br />
            など、まずはお気軽にお声掛けください。オンライン相談はその場で日時予約が可能です。
          </span>
        </div>
      </a>
    </div>
    <div class="f-btn02">
      <ul>
        <li>
          <a href="">
            <div class="btn-inner">
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
          <a href="">
            <div class="btn-inner">
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
          <a href="">
            <div class="btn-inner">
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
          <dd>People</dd>
        </dl>
        <dl>
          <dt>Who We Are</dt>
          <dd>People</dd>
        </dl>
        <dl>
          <dt>Who We Are</dt>
          <dd>People</dd>
        </dl>
        <dl>
          <dt>Who We Are</dt>
          <dd>People</dd>
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
    background-color: #e6da00;
    text-align: center;
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
        background: #2e334f;
        width: -webkit-calc(100% / 3);
        width: calc(100% / 3);
        position: relative;
        padding: 8rem 0;
        > a {
          color: $color-white;
          > .btn-inner {
            padding: 7rem 0;
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
    padding: 5rem 12rem;
    &__box {
      color: $color-white;
      display: flex;
      justify-content: space-between;
      > dl {
        width: -webkit-calc(100% / 4);
        width: calc(100% / 4);
        display: block;
        padding: 5rem 0;
        > dt {
          font-size: 1.9rem;
          font-weight: 700;
          margin-bottom: 2.5rem;
          > dd {
            font-size: 1.2rem;
            font-weight: 300;
          }
        }
      }
    }
  }
  .copylight{
    width: 100%;
    background-color: #12141d;
    >p{
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
    font-size: 2.4rem;
    padding: 0 0 3.8rem;
    display: block;
    font-weight: 900;
    // font-family: $font-midash;
  }
  .btn-text {
    font-size: 1.2rem;
    position: relative;
    display: inline-block;
    font-weight: 300;
    line-height: 2;
    letter-spacing: 0.05rem;
  }
  .btn-icon {
    margin-bottom: 2.8rem;
  }
}
</style>
