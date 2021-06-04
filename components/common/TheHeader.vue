<template>
	<header class="header">
		<div class="header-inner">
			<h1 class="logo"><a href=""><LogoSvg /></a></h1>
            <nav id="g-nav">
                <div id="g-nav-list">
                    <ul id="g-navi" class="nav">
                        <li><a href="#">About</a></li>
                        <li><a href="#">Works</a></li>
                        <li><a href="#">Findings</a></li>
                        <li><a href="#">Events</a></li>
                        <li><a href="#">People</a></li>
                        <li><a href="#">Contact</a></li>
                    </ul>
                </div>
                <div class=""></div>
            </nav>
		</div>
	</header>
</template>

<script>
import LogoSvg from '~/assets/svg/Logo.svg?inline';

export default {
  components: {
    LogoSvg
  },
}
</script>

<style lang="scss" scoped>
@import '~assets/scss/variables';

header{
    width: 100%;
    position: fixed;
    font-family: $font-header;
    font-weight: bold;
    .header-inner{
        width: 100%;
        height: 70px;
        z-index: 999;
        display: flex;
        justify-content: space-between;
        align-items: center;
        text-align: center;
        padding: 20px 100px 20px 0;
        .logo{
            text-transform: uppercase;
            padding: 0 0 0 2%;
            line-height: 1;
            white-space: nowrap;
        }
        #g-nav{
            &-list{
                .nav{
                    display: flex;
                    justify-content: center;
                    color: #000000;
                    li{
                    // color: $color-white;
                    color: #000000;
                    font-size: 1.5rem;
                    // text-align: center;
                        > a {
                            color: #eee;
                            padding: 50px 25px;
                            letter-spacing: 0.1rem;
                            transition: all .3s;
                        }
                    }
                }
            }
        }
    }
}
.header{
    height: 70px;
    width: 100%;
    z-index: 999;
    display: flex;
    justify-content: space-between;
    align-items: center;
    text-align: center;
    padding: 20px 100px 20px 0;
}
</style>
