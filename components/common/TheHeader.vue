<template>
	<header class="header">
		<div class="header-inner">
			<h1 class="logo"><LogoSvg /></h1>
            <div class="nav">
                <ul class="nav__inner">
                    <li class="nav__inner__name">About</li>
                    <li class="nav__inner__name">Works</li>
                    <li class="nav__inner__name">Findings</li>
                    <li class="nav__inner__name">Events</li>
                    <li class="nav__inner__name">People</li>
                    <li class="nav__inner__name">Contact</li>
                </ul>
                <div class=""></div>
            </div>
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
    font-family: $font-header;
    font-weight: bold;
    width: 100%;
    .header-inner{
        display: table;
        table-layout: fixed;
        width: 100%;
        .logo{
            display: table-cell;
            vertical-align: middle;
        }
        .nav{
            text-align: right;
            &__inner{
            display: table;
            table-layout: fixed;
            width: 600px;
            height: 150px;
                // display: flex;
                &__name{
                    display: table-cell;
                    vertical-align: middle;
                    // color: $color-white;
                    color: #000000;
                    font-size: 2.1rem;
                    text-align: center;
                }
            }
        }
    }
}
</style>
