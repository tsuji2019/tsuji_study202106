<template>
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
</template>

<script>
export default {
  components: {},

  mounted: function () {
    var slide = 0,
    slides = document.querySelectorAll('#slides > li'),
    numSlides = slides.length,

    //Functions!!
    currentSlide = function() {
      var itemToShow = Math.abs(slide % numSlides);
      [].forEach.call(slides, function(el) {
        el.classList.remove('slideActive')
      });
      slides[itemToShow].classList.add('slideActive');
      resetProgress();
      resetInterval();
    },
    next = function() {
      slide++;
      currentSlide();
    },
    prev = function() {
      slide--;
      currentSlide();
    },
    resetProgress = function() {
      var elm = document.querySelector('.progressbar'),
          newone = elm.cloneNode(true),
          x = elm.parentNode.replaceChild(newone, elm);
    },
    resetslide = function() {
      var elm = document.querySelector('#slides > li'),
          newone = elm.cloneNode(true),
          x = elm.parentNode.replaceChild(newone, elm);
    },
    resetInterval = function() {
      clearInterval(autonext);
      autonext = setInterval(function() {
        slide++;
        currentSlide();
      }, 10000);
    },
    autonext = setInterval(function() {
      next();
    }, 10000);


//Buttons
document.querySelector('#first').addEventListener('click', function() {
    slide = 0;
    currentSlide();
}, false);
document.querySelector('#second').addEventListener('click', function() {
    slide = 1;
    currentSlide();
}, false);
document.querySelector('#third').addEventListener('click', function() {
    slide = 2;
    currentSlide();
}, false);
document.querySelector('#fourth').addEventListener('click', function() {
    slide = 3;
    currentSlide();
}, false);
document.querySelector('#fifth').addEventListener('click', function() {
    slide = 4;
    currentSlide();
}, false);
document.querySelector('#sixth').addEventListener('click', function() {
    slide = 5;
    currentSlide();
}, false);
document.querySelector('#next').addEventListener('click', function() {
    next();
}, false);
document.querySelector('#previous').addEventListener('click', function() {
    prev();
}, false);
  },
};
</script>

<style lang="scss" scoped>
@import "~assets/scss/variables";

#slideshow{
	line-height: 1;
	font-family:Consolas, "Andale Mono", "Lucida Console", "Lucida Sans Typewriter", Monaco, "Courier New", monospace;
  position: relative;
  height: 100vh;
  width: 100vw;
}
.control {
	width: 100%;
	height: calc(100% - 36px);
	position: absolute;
	top:36px;
	margin: 0;
	z-index: 99;
  display: block;
}
.control > button {
	width: 16.7%;
	height: calc(100% - 36px);
	opacity: 1;
	color:#212121;
  background-color: transparent;
	border: 0;
  cursor: pointer;
  font-size: 50vh
}
#previous{
  float: left;
}
#next{
  float: right;
}
#slides {
	padding: 0;
	margin: 0;
	background: #000;
	overflow: hidden
}
#slides > li {
	position: absolute;
	clear:both;
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
	color:#212121;
}
#slides li:first-child {
	background: #F44336
}
#slides li:nth-child(2) {
	background: #E91E63
}
#slides li:nth-child(3) {
	background: #9C27B0
}
#slides li:nth-child(4) {
	background: #673AB7
}
#slides li:nth-child(5) {
	background: #3F51B5
}
#slides li:last-child {
	background: #2196F3
}
#slides li.slideActive {
	z-index: 2;
	opacity: 1;
	transition: 1s;
}
#first {
	background: #F44336
}
#second {
	background: #E91E63
}
#third {
	background: #9C27B0
}
#fourth {
	background: #673AB7
}
#fifth {
	background: #3F51B5
}
#sixth {
	background: #2196F3
}
.pager ul {
	display: table;
	width: 100%;
  position: absolute;
  z-index: 999
}
.pager ul li {
display: table-cell;
 line-height: 36px;
 text-align: center;
 color: #fff;
 text-decoration: none;
 cursor:pointer;
}
.progressbar{
	position:absolute;
	bottom: 0;
	width:100%;
	height:36px;
	background: none;
	z-index: 3;
}
.progress{
	width:0;
	height:36px;
	-webkit-animation: progress 10s infinite;
	background:#FFEB3B;
}
@-webkit-keyframes progress {
    0% {width: 0%;}
    100% {width: 100%;}
}
</style>