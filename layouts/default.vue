<template>
  <div id="allview">
    <TheHeader />
    <main class="contents">
      <nuxt />
    </main>
    <TheFooter />
  </div>
</template>

<script>
import TheHeader from "~/components/common/TheHeader";
import TheFooter from "~/components/common/TheFooter";

export default {
  components: {
    TheHeader,
    TheFooter,
  },
  mounted: function () {
    //★バーガーメニューを押すと
    $(".openbtn").click(function () {
      //ボタンがクリックされたら
      $(this).toggleClass("active"); //ボタン自身に activeクラスを付与し
      $("#g-nav2").toggleClass("panelactive"); //ナビゲーションにpanelactiveクラスを付与
      $("#allview").toggleClass("mainblur"); //ぼかしたいエリアにmainblurクラスを付与
    });
    $("#g-nav2 a").click(function () {
      //ナビゲーションのリンクがクリックされたら
      $(".openbtn").removeClass("active"); //除去
      $("#g-nav2").removeClass("panelactive"); //除去
      $("#allview").removeClass("mainblur"); //除去
    });
  },
};
</script>

<style lang="scss">
/* ナビゲーション */
#g-nav2 {
  position: fixed;
  z-index: -1;
  opacity: 0;
  top: 0;
  width: 100%;
  // height: 100vh;
  background: #262a42;
  transition: all 0.3s;
}
#g-nav2.panelactive {
  opacity: 1;
  z-index: 999;
  height: 100vh;
}
/*ナビゲーションの縦スクロール*/
#g-nav2.panelactive #g-nav2-list {
  position: fixed;
  z-index: 999;
  width: 100%;
  overflow: hidden;
  height: 100vh;
}

/*ナビゲーション*/
#g-nav2 ul {
  display: none;
  position: absolute;
  z-index: 999;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

#g-nav2.panelactive ul {
  display: block;
}

/*リストのレイアウト設定*/

#g-nav2 li {
  list-style: none;
  text-align: center;
}

#g-nav2 li a {
  color: #fff;
  text-decoration: none;
  padding: 10px;
  display: block;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  font-weight: bold;
}
/*========= ハンバーガーボタン ===============*/
.openbtn {
  position: fixed;
  z-index: 9999;
  right: 0;
  cursor: pointer;
  width: 11rem;
  height: 12.5rem;
}
.openbtn span {
  display: inline-block;
  transition: all 0.2s ease-out;
  -webkit-transition: all .2s ease-out;
  position: absolute;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
  margin: auto;
  background: #fff;
  width: 3rem;
  height: 0.4rem;
}

.openbtn span:nth-of-type(1) {
  top: -2.3rem;
}

.openbtn span:nth-of-type(2) {
  top: 0;
}

.openbtn span:nth-of-type(3) {
  top: 2rem;
}
.openbtn.active span:nth-of-type(1) {
  top: -1rem;
  left: 0;
  transform: translateY(6px) rotate(-45deg);
  width: 3rem;
}

.openbtn.active span:nth-of-type(2) {
  opacity: 0;
}

.openbtn.active span:nth-of-type(3) {
  top: 1.4rem;
  left: 0;
  transform: translateY(-6px) rotate(45deg);
  width: 3rem;
}
</style>