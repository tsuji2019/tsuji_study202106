<template>
  <div id="container">
    <div id="slideshow">
      <div class="control">
        <button id="previous">&lt;</button>
        <button id="next">&gt;</button>
      </div>
      <ul id="slides">
        <li class="slideActive">1</li>
        <li>2</li>
        <li>3</li>
        <li>4</li>
        <li>5</li>
        <li>6</li>
      </ul>
      <div class="pager">
        <ul>
          <li id="first">1</li>
          <li id="second">2</li>
          <li id="third">3</li>
          <li id="fourth">4</li>
          <li id="fifth">5</li>
          <li id="sixth">6</li>
        </ul>
      </div>
      <div class="progressbar">
        <div class="full">
          <div class="progress"></div>
        </div>
      </div>
    </div>
    <div class="visual">
      <div class="card-box">
        <div class="visual__controlbar js-target card">
          <p class="v-copyright">©2021 Loftwork Inc. All rights reserved</p>
        </div>
      </div>
    </div>
    <!-- スクロールバー -->
    <!-- <div class="">
      <p class=""></p>
    </div> -->
    <!-- section 01 -->
    <div id="contents">
      <div class="title">
        <h2>
          What We Do
          <span class="h2-small">Our Projects</span>
        </h2>
        <p class="copy">
          ロフトワークは今、何と向き合っているのか。現在進行形の旅と、少しだけ先の未来
        </p>
      </div>
      <div class="whatwedo">
        <ul class="whatwedo__list">
          <li class="whatwedo__list__item">
            <img src="~/assets/images/kv2.jpg" />
            <div class="whatwedo__list__item__ditail">
              <div class="tags">
                <p class="tag">
                  <span class="tag-bk">東大オリジナル株式会社</span>
                </p>
                <p class="tag"><span class="tag-gold">PROJECT</span></p>
              </div>
              <p class="item-title">
                ｢技術系｣＋｢人文系｣の可能性に切り込む 京大
                産学連携情報プラットフォーム｢Philo-｣(フィロ)構築
              </p>
              <span class="hashtag"><a href="#">#産官学連携</a></span>
              <span class="hashtag"><a href="#">#大学</a></span>
            </div>
          </li>
          <li class="whatwedo__list__item">
            <img src="~/assets/images/kv.jpg" />
            <div class="whatwedo__list__item__ditail">
              <div class="tags">
                <p class="tag">
                  <span class="tag-bk">東日本旅客鉄道株式会社</span>
                </p>
                <p class="tag"><span class="tag-gold">PROJECT</span></p>
              </div>
              <p class="item-title">
                モビリティ変革に、ユーザー視点を取り入れる。デザイン思考実践の場づくり
                NewHere Project
              </p>
              <span class="hashtag"><a href="#">#クリエイターとの共創</a></span>
              <span class="hashtag"><a href="#">#サービスデザイン</a></span>
              <span class="hashtag"><a href="#">#デザイン思考</a></span>
            </div>
          </li>
          <li class="whatwedo__list__item">
            <img src="~/assets/images/kv.jpg" />
            <div class="whatwedo__list__item__ditail">
              <div class="tags">
                <p class="tag"><span class="tag-bk">八尾市</span></p>
                <p class="tag"><span class="tag-gold">PROJECT</span></p>
              </div>
              <p class="item-title">
                はじめてのBtoCプロダクトづくり 八尾市の技術力を世界へ届けるYAOYA
                PROJECT2020
              </p>
              <span class="hashtag"><a href="#">#クリエイターとの共創</a></span>
              <span class="hashtag"><a href="#">#地方とデザイン</a></span>
              <span class="hashtag"><a href="#">#デザイン思考</a></span>
            </div>
          </li>
          <li class="whatwedo__list__item">
            <img src="~/assets/images/kv.jpg" />
            <div class="whatwedo__list__item__ditail">
              <div class="tags">
                <p class="tag"><span class="tag-bk">NTTレゾナント</span></p>
                <p class="tag"><span class="tag-gold">PROJECT</span></p>
              </div>
              <p class="item-title">
                新規事業アイデアのスケールを拡げる NTTレゾナント｢goo
                “未来ヒント”｣
              </p>
              <span class="hashtag"><a href="#">#事業開発</a></span>
              <span class="hashtag"><a href="#">#デザイン思考</a></span>
            </div>
          </li>
          <li class="whatwedo__list__item">
            <img src="~/assets/images/kv.jpg" />
            <div class="whatwedo__list__item__ditail">
              <div class="tags">
                <p class="tag"><span class="tag-bk">立命館大学</span></p>
                <p class="tag"><span class="tag-gold">PROJECT</span></p>
              </div>
              <p class="item-title">
                非接触時代の研修プログラムをデザイン
                オンライン研修開発ガイド｢PATHWAYS｣を制作・無償公開
              </p>
              <span class="hashtag"><a href="#">#事業開発</a></span>
              <span class="hashtag"><a href="#">#大学</a></span>
            </div>
          </li>
          <li class="whatwedo__list__item">
            <img src="~/assets/images/kv.jpg" />
            <div class="whatwedo__list__item__ditail">
              <div class="tags">
                <p class="tag">
                  <span class="tag-bk">株式会社ブリヂストン</span>
                </p>
                <p class="tag"><span class="tag-gold">PROJECT</span></p>
              </div>
              <p class="item-title">
                “人の動きを支える”ブリヂストンへ
                ソフトロボティクス事業にかける想い
              </p>
              <span class="hashtag"><a href="#">#対談・鼎談</a></span>
              <span class="hashtag"><a href="#">#事業開発</a></span>
              <span class="hashtag"><a href="#">#MTRL</a></span>
            </div>
          </li>
        </ul>
      </div>
      <a href="#" class="btn bgleft btn__plus"
        ><span class="btn-text">その他プロジェクトを見る</span></a
      >
    </div>

    <!-- section 02 -->
    <div id="contents">
      <div class="title title__center">
        <h2 class="h2-center">
          <span class="h2-small">Pickup Contents</span>
          Events<span class="slashーsmall">/</span>News<span
            class="slashーsmall"
            >/</span
          >Columns
        </h2>
      </div>
      <div class="pickup">
        <ul class="pickup__list">
          <li class="pickup__list__item">
            <img src="~/assets/images/kv.jpg" />
            <div class="pickup__list__item__ditail">
              <div class="tags">
                <p class="tag"><span class="tag-gold">EVENT</span></p>
                <p class="tag">
                  <span class="fs--12 fw--700">オンライン</span>
                </p>
              </div>
              <p class="item-title">
                「手に取る機会を取り戻す」コミュニケーションツールのデザイン ー
                事例：東レ ウルトラスエード x 1518
              </p>
              <span class="hashtag-number">2021.0602</span>
              <span class="hashtag"><a href="#">#大学</a></span>
            </div>
          </li>
          <li class="pickup__list__item">
            <img src="~/assets/images/kv.jpg" />
            <div class="pickup__list__item__ditail">
              <div class="tags">
                <p class="tag"><span class="tag-gold">EVENT</span></p>
                <p class="tag">
                  <span class="fs--12 fw--700"
                    >オンライン（zoom）＋オフライン開催</span
                  >
                </p>
              </div>
              <p class="item-title">
                [SMBCグループ・ロフトワーク共催]
                寄付のデザイン−寄付から生まれるサステナブルな社会とは？
              </p>
              <span class="hashtag-number">2021.0602</span>
            </div>
          </li>
          <li class="pickup__list__item">
            <img src="~/assets/images/kv.jpg" />
            <div class="pickup__list__item__ditail">
              <div class="tags">
                <p class="tag"><span class="tag-gold">EVENT</span></p>
                <p class="tag">
                  <span class="fs--12 fw--700">オンライン+名古屋</span>
                </p>
              </div>
              <p class="item-title">
                組織変革をデザインするための公開相談会 ー
                元マッキンゼー東京支社長、横山禎徳氏に学ぶ
              </p>
              <span class="hashtag-number">2021.0601</span>
              <span class="hashtag"><a href="#">#デザイン経営</a></span>
              <span class="hashtag"><a href="#">#デザインリサーチ</a></span>
            </div>
          </li>
          <li class="pickup__list__item">
            <img src="~/assets/images/kv.jpg" />
            <div class="pickup__list__item__ditail">
              <div class="tags">
                <p class="tag"><span class="tag-gold">EVENT</span></p>
                <p class="tag">
                  <span class="fs--12 fw--700">オンライン</span>
                </p>
              </div>
              <p class="item-title">
                エシカル暮らすメイト 7Days Challenge #DAY0 KICKOFF
                エシカルな暮らしはどうできる？活動前夜に語らう。
              </p>
              <span class="hashtag-number">2021.0520</span>
              <span class="hashtag"><a href="#">#SDGs / ESG</a></span>
            </div>
          </li>
          <li class="pickup__list__item">
            <img src="~/assets/images/kv.jpg" />
            <div class="pickup__list__item__ditail">
              <div class="tags">
                <p class="tag"><span class="tag-gold">EVENT</span></p>
                <p class="tag">
                  <span class="fs--12 fw--700">オンライン</span>
                </p>
              </div>
              <p class="item-title">
                「女性発の新事業」を阻む4つの壁とは？
                誰もが輝くための場づくりとルールメイキング
              </p>
              <span class="hashtag-number">2021.0518</span>
              <span class="hashtag"><a href="#">#SDGs / ESG</a></span>
              <span class="hashtag"><a href="#">#事業開発</a></span>
              <span class="hashtag"><a href="#">#サービスデザイン</a></span>
            </div>
          </li>
          <li class="pickup__list__item">
            <img src="~/assets/images/kv.jpg" />
            <div class="pickup__list__item__ditail">
              <div class="tags">
                <p class="tag"><span class="tag-gold">EVENT</span></p>
                <p class="tag">
                  <span class="fs--12 fw--700">オンライン</span>
                </p>
              </div>
              <p class="item-title">
                Dcraft デザイン経営リーダーズゼミ 成果報告会
              </p>
              <span class="hashtag-number">2021.0525</span>
              <span class="hashtag"><a href="#">##デザイン経営</a></span>
              <span class="hashtag"><a href="#">#Project-OnGoing</a></span>
              <span class="hashtag"><a href="#">#ブランド体験</a></span>
            </div>
          </li>
        </ul>
      </div>
      <div class="btn-viewmore">
        <div class="btn-inner">
          <a href=""><span>もっと見る</span></a>
        </div>
      </div>
      <a href="#" class="btn bgleft btn__plus"
        ><span class="btn-text">その他プロジェクトを見る</span></a
      >
    </div>

    <!-- section 03 -->
    <div id="contents">
      <div class="title">
        <h2>
          How We Work
          <span class="h2-small">Findings ＆ Methods</span>
        </h2>
        <p class="copy">
          私たちの考えかた、つくりかた。未知を探索する旅の途上で見つけた“創造性の種”
        </p>
      </div>
      <div class="works">
        <div class="works__slide">
          <img src="~/assets/images/kv.jpg" />
        </div>
        <div class="works__list">
          <!-- works left -->
          <div class="works__list__inner">
            <ul class="works__list__left">
              <li class="works__list__left__item">
                <ul class="left-inner">
                  <li class="thumb01">
                    <img src="~/assets/images/kv.jpg" />
                  </li>
                  <li class="text01">
                    <span class="hashtag-number">2021.06.02</span>
                    <p class="item-title">
                      ええ空気を探して vol.1<br />
                      テクノロジーの研究者と探る場作りのヒント<br />
                      (現代アーティスト/研究者 川端 渉)
                    </p>
                    <p class="look-icon"><span></span>104</p>
                    <span class="hashtag"><a href="#">#対談・鼎談</a></span>
                    <span class="hashtag"><a href="#">#COUNTER POINT</a></span>
                    <span class="hashtag"><a href="#">#空間デザイン</a></span>
                  </li>
                </ul>
              </li>
            </ul>
            <div class="btn-viewmore">
              <div class="btn-inner">
                <a href="#" class="btn2 bgleft"><span>もっと見る</span></a>
              </div>
            </div>
          </div>
          <!-- works right -->
          <div class="works__list__right">
            <p class="works__list__right__title">Popular Post</p>
            <ul class="works__list__right__inner">
              <li>
                <ul class="right-inner">
                  <li class="thumb02">
                    <img src="~/assets/images/kv.jpg" />
                  </li>
                  <li class="text02">
                    <span class="hashtag-name">鈴木 真理子</span>
                    <p class="look-icon"><span></span>104</p>
                    <p class="item-title">
                      ボトムアップで始まった、ロフトワークの“創造的な組織づくり”<br />
                      「NANDA会」レポート
                    </p>
                  </li>
                </ul>
              </li>
            </ul>
          </div>
        </div>
      </div>
      <a href="#" class="btn bgleft btn__plus">
        <span class="btn-text">How We Work 詳しくはこちら</span>
      </a>
    </div>

    <!-- section 04 -->
    <div id="contents">
      <div class="accsess">
        <!-- accsess left -->
        <div class="accsess__slide">
          <img src="~/assets/images/kv.jpg" />
        </div>
        <!-- accsess right -->
        <div class="accsess__list">
          <!-- accsess right -->
          <div class="accsess__list__right">
            <p class="accsess__list__right__title">Popular Post</p>
            <ul class="accsess__list__right__inner">
              <li>
                <ul class="right-inner">
                  <li class="thumb02">
                    <img src="~/assets/images/kv.jpg" />
                  </li>
                  <li class="text02">
                    <span class="hashtag-name">鈴木 真理子</span>
                    <p class="look-icon"><span></span>104</p>
                    <p class="item-title">
                      ボトムアップで始まった、ロフトワークの“創造的な組織づくり”<br />
                      「NANDA会」レポート
                    </p>
                  </li>
                </ul>
              </li>
            </ul>
          </div>
        </div>
      </div>
      <a href="#" class="btn bgleft btn__plus">
        <span class="btn-text">How We Work 詳しくはこちら</span>
      </a>
    </div>

    <!-- // 動作確認コード
    <div class="hoge1">
      このテキストは青くなりますこのテキストは青くなります
    </div> -->
  </div>
</template>

<script>
export default {
  components: {},

  mounted: function () {
    var slide = 0,
      slides = document.querySelectorAll("#slides > li"),
      numSlides = slides.length,
      //Functions!!
      currentSlide = function () {
        var itemToShow = Math.abs(slide % numSlides);
        [].forEach.call(slides, function (el) {
          el.classList.remove("slideActive");
        });
        slides[itemToShow].classList.add("slideActive");
        resetProgress();
        resetInterval();
      },
      next = function () {
        slide++;
        currentSlide();
      },
      prev = function () {
        slide--;
        currentSlide();
      },
      resetProgress = function () {
        var elm = document.querySelector(".progressbar"),
          newone = elm.cloneNode(true),
          x = elm.parentNode.replaceChild(newone, elm);
      },
      resetslide = function () {
        var elm = document.querySelector("#slides > li"),
          newone = elm.cloneNode(true),
          x = elm.parentNode.replaceChild(newone, elm);
      },
      resetInterval = function () {
        clearInterval(autonext);
        autonext = setInterval(function () {
          slide++;
          currentSlide();
        }, 10000);
      },
      autonext = setInterval(function () {
        next();
      }, 10000);

    //Buttons
    document.querySelector("#first").addEventListener(
      "click",
      function () {
        slide = 0;
        currentSlide();
      },
      false
    );
    document.querySelector("#second").addEventListener(
      "click",
      function () {
        slide = 1;
        currentSlide();
      },
      false
    );
    document.querySelector("#third").addEventListener(
      "click",
      function () {
        slide = 2;
        currentSlide();
      },
      false
    );
    document.querySelector("#fourth").addEventListener(
      "click",
      function () {
        slide = 3;
        currentSlide();
      },
      false
    );
    document.querySelector("#fifth").addEventListener(
      "click",
      function () {
        slide = 4;
        currentSlide();
      },
      false
    );
    document.querySelector("#sixth").addEventListener(
      "click",
      function () {
        slide = 5;
        currentSlide();
      },
      false
    );
    document.querySelector("#next").addEventListener(
      "click",
      function () {
        next();
      },
      false
    );
    document.querySelector("#previous").addEventListener(
      "click",
      function () {
        prev();
      },
      false
    );

    // ヴィジュアル下のコントロールバーを倒す
    const map = (val, inputMin, inputMax, outputMin, outputMax) => {
      if (val <= inputMin) return false;
      if (val >= inputMax) return false;
      const p = (outputMax - outputMin) / (inputMax - inputMin);
      return (val - inputMin) * p + outputMin;
    };
    let target;
    let windowHeight;
    let windowHalfY;

    const handleScroll = () => {
      const scrollY = window.scrollY;
      const val = map(scrollY, windowHalfY, windowHeight, 0, 95);
      target.style.transform = `rotateX(${val}deg)`;
    };
    const resize = () => {
      windowHeight = window.innerHeight;
      windowHalfY = windowHeight / 2;
    };
    const handleResize = () => {
      resize();
    };
    const init = () => {
      target = document.querySelector(".js-target");
      resize();

      window.addEventListener("scroll", handleScroll);
      window.addEventListener("resize", handleResize);
    };
    init();
  },
};
</script>

<style lang="scss" scoped>
@import "~assets/scss/variables";
// 動作確認コード
// .hoge1{
// color:#999;
// }

#container {
  margin: 0 auto;
  width: 100%;
  height: 100%;
  overflow: hidden;
}
.visual {
  // position: relative;
  &__controlbar {
    min-width: 100rem;
    width: 110rem;
    height: 6.6rem;
    background-color: $color-white;
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    margin: 0 auto;
    .v-copyright {
      font-family: $font-accent;
      color: $color-black;
      margin: auto;
      text-align: left;
      font-weight: 400;
      font-size: 1rem;
      font-style: italic;
      display: inline-block;
      padding: 2.9rem 0;
      padding-left: 2.8rem;
    }
  }
}

#contents {
  margin: auto;
  // margin-bottom: 500px;
  // padding: 0 10rem;
  // width: 1000px;

  // h2 タイトル
  .title {
    margin: 60px auto;
    display: table;
    table-layout: fixed;
    width: 100%;
    min-width: 1000px;
    padding: 0 10rem;
    h2 {
      display: table-cell;
      vertical-align: middle;
      font-family: $font-h2;
      font-weight: bold;
      font-size: 2.8em;
      padding-right: 5rem;
      width: 20%;
      .h2-small {
        font-family: $font-accent;
        color: $color-ylw-100;
        font-weight: 400;
        font-size: 1.2rem;
        display: block;
        padding-top: 1.8rem;
      }
    }
    .copy {
      font-size: 1.4rem;
      font-weight: 200;
      display: table-cell;
      vertical-align: middle;
      border-left: 1px solid $color-lightgray;
      width: 80%;
      padding-left: 5rem;
    }
  }
  .title__center {
    text-align: center;
    padding: 0;
    margin-top: 6rem;
    margin-bottom: 6rem;
    .h2-center {
      text-align: center;
      padding: 0;
      > span {
        padding-bottom: 2rem;
      }
      .slashーsmall {
        font-size: 1.8rem;
        font-weight: 400;
        margin-bottom: 1.8rem;
        padding: 0 1rem;
      }
    }
  }
  .whatwedo {
    width: 100%;
    min-width: 1000px;
    &__list {
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      flex-flow: row wrap;
      padding: 0 10rem;
      &__item {
        width: -webkit-calc(336 / 1080 * 100%);
        width: calc(336 / 1080 * 100%);
        font-family: $font-text;
        font-weight: 100;
        margin-bottom: 68px;
        &__ditail {
          margin-top: 28px;
          .tags {
            margin-bottom: 16px;
          }
          .item-title {
            font-size: 1.9rem;
            font-weight: 900;
            line-height: 1.6;
            color: $color-black;
            margin-bottom: 22px;
          }
        }
        .hashtag {
          a {
            &:hover {
              color: #8d7b00;
              text-decoration: underline;
            }
          }
        }
      }
    }
  }
  .pickup {
    width: 100%;
    min-width: 1000px;
    position: relative;
    &__list {
      position: relative;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      flex-flow: row wrap;
      padding: 0 10rem;
      &__item {
        width: -webkit-calc(100% / 3);
        width: calc(100% / 3);
        font-family: $font-text;
        font-weight: 100;
        border-bottom: 1px solid rgba(0, 0, 0, 0.05);
        &__ditail {
          margin: 4.8rem 3.8rem 5.6rem;
          .tags {
            margin-bottom: 1.6rem;
          }
          .item-title {
            font-size: 1.9rem;
            font-weight: 900;
            line-height: 1.6;
            color: $color-black;
            margin-bottom: 22px;
          }
        }
        .hashtag {
          a {
            &:hover {
              color: #8d7b00;
              text-decoration: underline;
              font-weight: 500;
            }
          }
        }
        .hashtag-number {
          font-size: 1.2rem;
          color: #ccc;
          padding-right: 1.2rem;
        }
      }
    }
  }
  .btn-viewmore {
    text-align: center;
    padding: 6rem 0 12rem;
  }

  // contents works
  .works {
    &__slide {
      padding: 0 10rem;
      margin-bottom: 8rem;
    }
    &__list {
      display: -webkit-flex;
      display: flex;
      -webkit-justify-content: space-between;
      justify-content: space-between;
      margin: 0 auto;
      padding: 0 10rem;
      // works left
      &__inner {
        width: 72%;
        .works__list__left {
          width: 100%;
          display: -webkit-flex;
          display: flex;
          -webkit-justify-content: space-between;
          justify-content: space-between;
          &__item {
            position: relative;
            padding: 0 1rem;
            .left-inner {
              display: -webkit-flex;
              display: flex;
              -webkit-justify-content: space-between;
              justify-content: space-between;
              margin: 5rem auto;
              .thumb01 {
                width: 35.5%;
              }
              .text01 {
                width: 59%;
                font-family: $font-text;
                .hashtag-number {
                  color: $color-lightgray;
                  font-weight: 400;
                  font-size: 1.2rem;
                  letter-spacing: 0.1rem;
                }
                .item-title {
                  font-size: 2.2rem;
                  line-height: 1.6;
                  color: #1a1a1a;
                  font-weight: 900;
                  margin: 2rem 0;
                }
                .look-icon {
                  display: inline-block;
                  vertical-align: middle;
                  font-size: 1.3rem;
                  letter-spacing: 0.05em;
                  font-family: quasimoda, sans-serif;
                  font-weight: 800;
                  margin-right: 1rem;
                }
              }
            }
            &::before,
            &::after {
              content: "";
              display: block;
              width: 100%;
              height: 0.1rem;
            }
            &::before {
              background-color: $color-lightgray;
              position: absolute;
              top: 0;
              left: 0;
            }
            &::after {
              background-color: $color-lightgray;
              position: absolute;
              bottom: 0;
              left: 0;
            }
          }
        }
      }
      &__right {
        width: 23%;
        height: auto;
        position: relative;
        &__title {
          font-family: $font-accent;
          padding: 1.8rem 0;
          text-align: center;
          background-color: #f7f6f2;
          color: $color-black;
          font-size: 1.4rem;
          font-weight: 100;
        }
        &__inner {
          > li {
            position: relative;
            .right-inner {
              display: -webkit-flex;
              display: flex;
              -webkit-justify-content: space-between;
              justify-content: space-between;
              padding: 2.6rem 0;
              .thumb02 {
                width: 28%;
              }
              .text02 {
                width: 67%;
                font-family: $font-text;
                .hashtag-name {
                  color: $color-lightgray;
                  font-weight: 400;
                  font-size: 1rem;
                  letter-spacing: 0.1rem;
                  color: $color-lightgray;
                }
                .item-title {
                  font-size: 1.1rem;
                  line-height: 1.8;
                  color: #1a1a1a;
                  font-weight: 900;
                  margin: 1.3rem 0;
                }
                > .look-icon {
                  display: inline-block;
                  vertical-align: middle;
                  float: right;
                  font-size: 1rem;
                  letter-spacing: 0.05em;
                  font-family: quasimoda, sans-serif;
                  font-weight: 800;
                  margin-right: 1rem;
                }
              }
            }
            &::after {
              content: "";
              display: block;
              width: 100%;
              height: 0.1rem;
              background-color: $color-lightgray;
              position: absolute;
              bottom: 0;
              left: 0;
            }
          }
        }
        &::before,
        &::after {
          content: "";
          display: block;
          width: 100%;
          height: 0.1rem;
        }
        &::before {
          background-color: $color-lightgray;
          position: absolute;
          top: 0;
          left: 0;
        }
        &::after {
          background-color: $color-lightgray;
          position: absolute;
          bottom: 0;
          left: 0;
        }
      }
    }
  }
  // contents accsess
  .accsess {
    &__slide {
      padding: 0 10rem;
      margin-bottom: 8rem;
    }
    &__list {
      display: -webkit-flex;
      display: flex;
      -webkit-justify-content: space-between;
      justify-content: space-between;
      margin: 0 auto;
      padding: 0 10rem;
      // accsess left
      &__inner {
        width: 72%;
        .accsess__list__left {
          width: 100%;
          display: -webkit-flex;
          display: flex;
          -webkit-justify-content: space-between;
          justify-content: space-between;
          &__item {
            position: relative;
            padding: 0 1rem;
            .left-inner {
              display: -webkit-flex;
              display: flex;
              -webkit-justify-content: space-between;
              justify-content: space-between;
              margin: 5rem auto;
              .thumb01 {
                width: 35.5%;
              }
              .text01 {
                width: 59%;
                font-family: $font-text;
                .hashtag-number {
                  color: $color-lightgray;
                  font-weight: 400;
                  font-size: 1.2rem;
                  letter-spacing: 0.1rem;
                }
                .item-title {
                  font-size: 2.2rem;
                  line-height: 1.6;
                  color: #1a1a1a;
                  font-weight: 900;
                  margin: 2rem 0;
                }
                .look-icon {
                  display: inline-block;
                  vertical-align: middle;
                  font-size: 1.3rem;
                  letter-spacing: 0.05em;
                  font-family: quasimoda, sans-serif;
                  font-weight: 800;
                  margin-right: 1rem;
                }
              }
            }
            &::before,
            &::after {
              content: "";
              display: block;
              width: 100%;
              height: 0.1rem;
            }
            &::before {
              background-color: $color-lightgray;
              position: absolute;
              top: 0;
              left: 0;
            }
            &::after {
              background-color: $color-lightgray;
              position: absolute;
              bottom: 0;
              left: 0;
            }
          }
        }
      }
      &__right {
        width: 23%;
        height: auto;
        position: relative;
        &__title {
          font-family: $font-accent;
          padding: 1.8rem 0;
          text-align: center;
          background-color: #f7f6f2;
          color: $color-black;
          font-size: 1.4rem;
          font-weight: 100;
        }
        &__inner {
          > li {
            position: relative;
            .right-inner {
              display: -webkit-flex;
              display: flex;
              -webkit-justify-content: space-between;
              justify-content: space-between;
              padding: 2.6rem 0;
              .thumb02 {
                width: 28%;
              }
              .text02 {
                width: 67%;
                font-family: $font-text;
                .hashtag-name {
                  color: $color-lightgray;
                  font-weight: 400;
                  font-size: 1rem;
                  letter-spacing: 0.1rem;
                  color: $color-lightgray;
                }
                .item-title {
                  font-size: 1.1rem;
                  line-height: 1.8;
                  color: #1a1a1a;
                  font-weight: 900;
                  margin: 1.3rem 0;
                }
                > .look-icon {
                  display: inline-block;
                  vertical-align: middle;
                  float: right;
                  font-size: 1rem;
                  letter-spacing: 0.05em;
                  font-family: quasimoda, sans-serif;
                  font-weight: 800;
                  margin-right: 1rem;
                }
              }
            }
            &::after {
              content: "";
              display: block;
              width: 100%;
              height: 0.1rem;
              background-color: $color-lightgray;
              position: absolute;
              bottom: 0;
              left: 0;
            }
          }
        }
        &::before,
        &::after {
          content: "";
          display: block;
          width: 100%;
          height: 0.1rem;
        }
        &::before {
          background-color: $color-lightgray;
          position: absolute;
          top: 0;
          left: 0;
        }
        &::after {
          background-color: $color-lightgray;
          position: absolute;
          bottom: 0;
          left: 0;
        }
      }
    }
  }
  .pickup__list__item::before,
  .pickup__list__item::after {
    content: "";
    z-index: -1;
    position: absolute;
    top: 0;
    display: block;
    width: 1px;
    height: 100%;
    background: rgba(0, 0, 0, 0.05);
  }
  .pickup__list__item::after {
    right: 10rem;
    opacity: 0.4;
  }
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}

// ヴィジュアル下のバーを倒す
/* 下へ */
.card-box {
  perspective: 60rem;
}
.card-box .js-target {
  transform-origin: 50% 100%;
}
// スライダー
#slideshow {
  line-height: 1;
  font-family: Consolas, "Andale Mono", "Lucida Console",
    "Lucida Sans Typewriter", Monaco, "Courier New", monospace;
  position: relative;
  height: 100vh;
  width: 100vw;
}
.control {
  width: 100%;
  height: calc(100% - 36px);
  position: absolute;
  top: 36px;
  margin: 0;
  z-index: 99;
  display: block;
}
.control > button {
  width: 16.7%;
  height: calc(100% - 36px);
  opacity: 1;
  color: #212121;
  background-color: transparent;
  border: 0;
  cursor: pointer;
  font-size: 50vh;
}
#previous {
  float: left;
}
#next {
  float: right;
}
#slides {
  padding: 0;
  margin: 0;
  background: #000;
  overflow: hidden;
}
#slides > li {
  position: absolute;
  clear: both;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  width: 100%;
  height: 100%;
  margin: 0 auto;
  overflow: hidden;
  opacity: 0;
  overflow: hidden;
  font-size: 50vh;
  line-height: 100vh;
  text-align: center;
  color: #212121;
}
#slides li:first-child {
  background: #f44336;
}
#slides li:nth-child(2) {
  background: #e91e63;
}
#slides li:nth-child(3) {
  background: #9c27b0;
}
#slides li:nth-child(4) {
  background: #673ab7;
}
#slides li:nth-child(5) {
  background: #3f51b5;
}
#slides li:last-child {
  background: #2196f3;
}
#slides li.slideActive {
  z-index: 2;
  opacity: 1;
  transition: 1s;
}
#first {
  background: #f44336;
}
#second {
  background: #e91e63;
}
#third {
  background: #9c27b0;
}
#fourth {
  background: #673ab7;
}
#fifth {
  background: #3f51b5;
}
#sixth {
  background: #2196f3;
}
.pager ul {
  display: table;
  width: 100%;
  position: absolute;
  z-index: 999;
}
.pager ul li {
  display: table-cell;
  line-height: 36px;
  text-align: center;
  color: #fff;
  text-decoration: none;
  cursor: pointer;
}
.progressbar {
  position: absolute;
  bottom: 0;
  width: 100%;
  height: 36px;
  background: none;
  z-index: 3;
}
.progress {
  width: 0;
  height: 36px;
  -webkit-animation: progress 10s infinite;
  background: #ffeb3b;
}
@-webkit-keyframes progress {
  0% {
    width: 0%;
  }
  100% {
    width: 100%;
  }
}
</style>
