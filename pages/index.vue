<template>
  <div class="container">
    <div>
      <div class="kv">
        <img src="~/assets/images/kv.jpg" />
      </div>
      <div id="contents01">
        <div>
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
                <li>
                  <img src="~/assets/images/kv.jpg" />
                  <div class="title"></div>
                  <p class="text"></p>
                  <span class="tag"></span>
                </li>
              </ul>
            </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "~assets/scss/variables";

.container {
  margin: 0 auto;
  width: 100%;
  max-width: 1280px;
  overflow: hidden;
  // min-height: 100vh;
  // display: flex;
  // justify-content: center;
  // align-items: center;
  // text-align: center;
}
.kv {
  img {
    width: 100%;
  }
}

#contents01 {
  margin: auto;
  margin-bottom: 500px;
  padding: 0 10rem;
  // width: 1000px;

  .title {
    margin: 60px auto;
    display: table;
    table-layout: fixed;
    width: 100%;
    h2 {
      display: table-cell;
      vertical-align: middle;
      font-family: $font-h2;
      font-weight: bold;
      font-size: 2.8em;
      padding-right: 5rem;
      width: 20%;
    }
    .h2-small {
      font-family: $font-h2-small;
      color: #c0a700;
      font-weight: 400;
      font-size: 1.2rem;
      display: block;
      padding-top: 1.8rem;
    }
    .copy {
      font-size: 1.4rem;
      display: table-cell;
      vertical-align: middle;
      border-left: 1px solid #e5e5e5;
      width: 80%;
      padding-left: 5rem;
    }
  }
  .whatwedo {
    width: 100%;
    margin: 0 auto;
    &__list{
      display: flex;
      justify-content: space-between;
      flex-flow: row wrap;
    }
  }
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px
}

.links {
  padding-top: 15px;
}
</style>
