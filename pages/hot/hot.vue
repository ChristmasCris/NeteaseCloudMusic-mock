<template>
	<view class="hot-container">
		<!--myBannerStart-->
		<my-banner/>
		<!--myBannerEnd-->
		<!--searchStart-->
		<view class="search">
			<my-search placeholder="每日推荐"/>
		</view>
		<!--serchEnd-->
		<!--首页发现Start-->
		<view class="my-scrolls">
			<scroll-view class="my-scroll" scroll-x="true" show-scrollbar="false" scroll-with-animation>
				<view class="my-scroll-view">
					<image class="scroll-image" src="https://p1.music.126.net/Shi7cRT1bDhwpVDM7AOFXg==/109951165265330616.jpg"
					       alt=""/>
					<view class="scroll-text">每日推荐</view>
				</view>
				<view class="my-scroll-view">
					<image class="scroll-image" src="https://p1.music.126.net/Shi7cRT1bDhwpVDM7AOFXg==/109951165265330616.jpg"
					       alt=""/>
					<view class="scroll-text">私人FM</view>
				</view>
				<view class="my-scroll-view">
					<image class="scroll-image" src="https://p1.music.126.net/uG5p6CnwAHrLqOkaSeRlnA==/109951163986649164.jpg"
					       alt=""/>
					<view class="scroll-text">歌单</view>
				</view>
				<view class="my-scroll-view">
					<image class="scroll-image" src="https://p1.music.126.net/SDFC6A3X2wzUCavYyeGIOg==/109951163986649670.jpg"
					       alt=""/>
					<view class="scroll-text">排行榜</view>
				</view>
				<view class="my-scroll-view">
					<image class="scroll-image" src="https://p1.music.126.net/2JvVZZjcjyCE72fGMsC1hg==/109951166989043011.jpg"
					       alt=""/>
					<view class="scroll-text">直播</view>
				</view>
				<view class="my-scroll-view">
					<image class="scroll-image" src="https://p1.music.126.net/yfJ57hKHTAt4YXJ6nGHpNw==/109951165923269139.jpg"
					       alt=""/>
					<view class="scroll-text">助眠解压</view>
				</view>
			</scroll-view>
			<!--首页发现End-->
			<!--首页发现End-->
			<view class="online"></view>
			<!--推荐歌单Start-->
			<view class="my-scroll-hot">
				<view class="list-text">推荐歌单</view>
				<scroll-view class="my-scroll-view-hot" scroll-x="true" show-scrollbar="false" scroll-with-animation>
					<view class="recommendedPlaylist">
						<image class="playListImg" src="https://p2.music.126.net/GzAAXJOnucWYfUGNIvrrlg==/109951166461327222.jpg"
						       alt=""/>
						<view class="playListText">日子需要我们积极向上</view>
					</view>
					<view class="recommendedPlaylist">
						<image class="playListImg" src="https://p1.music.126.net/rlsdhQC8HqhsRONS6OTnWA==/109951165802776639.jpg"
						       alt=""/>
						<view class="playListText">把普通的日子过浪漫些，我的意思是和你</view>
					</view>
					<view class="recommendedPlaylist">
						<image class="playListImg" src="https://p1.music.126.net/VdJLRajqqcxno2S3Mcbebg==/109951165914479717.jpg"
						       alt=""/>
						<view class="playListText">我想你了 其实我也很脆弱</view>
					</view>
					<view class="recommendedPlaylist">
						<image class="playListImg" src="https://p1.music.126.net/fob5pHV3xzGlJ_-KEeLFLg==/109951165693966983.jpg"
						       alt=""/>
						<view class="playListText">全网流行热歌（持续更新）</view>
					</view>
					<view class="recommendedPlaylist">
						<image class="playListImg" src="https://p1.music.126.net/xSei1yJKuSJY3sMFUkiYZg==/109951166924151597.jpg"
						       alt=""/>
						<view class="playListText">那些听了让人心情好的歌❤</view>
					</view>
				</scroll-view>
			</view>
			<!--推荐歌单End-->
		</view>
	</view>
</template>

<script>
import MySearch from "../../components/my-search/my-search";
import MyBanner from "../../components/my-banner/my-banner";

export default {
	components: {MyBanner, MySearch},
	data() {
		return {};
	},
	OnLoad() {
		//请求
	}
}
</script>
<style lang="scss" scoped>
.search {
	padding-top: 25rpx;
}

.hot-container {
	background-color: #fff;

	.logo {
		width: 100%;
		height: 80px;
	}

	.my-scrolls {
		padding: 25rpx 20rpx;
		width: 100%;
	}

	.my-scroll {
		width: 100%;
		white-space: nowrap;
	}
	.scroll-text{
		font-size: 14px;
	}
	.my-scroll-view {
		width: 150rpx;
		display: inline-block;
		text-align: center;

		.scroll-image {
			width: 88rpx;
			height: 88rpx;
			background: #ec6660;
			border-radius: 50%;
		}
	}

	.online {
		width: 100%;
		margin: 20rpx auto;
		border-bottom: 1rpx solid rgba(192, 192, 192, 0.5);
	}

	.list-text {
		font-size: 20px;
		font-weight: bold;
	}

	.my-scroll-view-hot {
		padding-top: 15rpx;
		white-space: nowrap;
	}

	.recommendedPlaylist {
		padding: 0 15rpx;
		width: 214rpx;
		height: 278rpx;
		display: inline-block;
	}

	.playListImg {
		width: 100%;
		height: 214rpx;
		border-radius: 15rpx;
	}
	.playListText{
		//文字自动换行
		white-space:normal;
		overflow: hidden;
		text-overflow: ellipsis;
		display:-webkit-box; //作为弹性伸缩盒子模型显示。
		-webkit-box-orient:vertical; //设置伸缩盒子的子元素排列方式--从上到下垂直排列
		-webkit-line-clamp:2; //显示的行
		text-align: center;
		font-size: 14px;
	}
}
</style>

