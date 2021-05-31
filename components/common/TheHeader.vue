<template>
	<header class="header">
		<div class="header-inner">
			<h1><LogoSvg /></h1>
            <div class="header-inner__nav">
                <ul class="header-inner__nav-inner">
                    <li class="header-inner__nav-inner__name">About</li>
                    <li class="header-inner__nav-inner__name">Works</li>
                    <li class="header-inner__nav-inner__name">Findings</li>
                    <li class="header-inner__nav-inner__name">Events</li>
                    <li class="header-inner__nav-inner__name">People</li>
                    <li class="header-inner__nav-inner__name">Contact</li>
                </ul>
                <div class=""></div>
            </div>
		</div>
	</header>
</template>

<script>
import LogoSvg from '@/assets/svg/Logo.svg';

export default {
  components: {
    LogoSvg,
  },
}
</script>

<style lang="scss" scoped>
@import '~assets/scss/variables';

header{
    font-family: $font-header;
    font-weight: bold;
    width: 100%;
}
</style>
