<template>
	<view class="banner">
		<swiper class="banner-swiper" indicator-dots="true" autoplay="true" vertical="true" indicator-active-color="#ffffff">
			<swiper-item>
				<image class="banner-img" src="https://p1.music.126.net/bTtIlpTcsWH0I7K_ol4d7Q==/109951167035498239.jpg"/>
			</swiper-item><swiper-item>
				<image class="banner-img" src="https://p1.music.126.net/rLJx73ilGPCg1tAOVtKOqQ==/109951167033033967.jpg"/>
			</swiper-item><swiper-item>
				<image class="banner-img" src="https://p1.music.126.net/cb2_pkQHmNtJOeanabuAAg==/109951167036127383.jpg"/>
			</swiper-item>
		</swiper>
	</view>
</template>

<script>
	export default {
		name:"my-banner",
		data() {
			return {

			};
		}
	}
</script>

<style lang="scss">
.banner{
	height:270rpx;
	margin:0 30rpx;
}
.banner-img{
	width:100%;
	height: 100%;
	border-radius: 20rpx;

}
</style>
