<template>
	<view class="search">
		<view class="search-container">
			<image class="search-image" src="@/static/images/search.png"/>
			<view class="search-placeholder">{{ placeholder }}</view>
		</view>
	</view>
</template>

<script>
export default {
	name: "my-search",
	props: {
		placeholder: {
			type: String,
			default: "请输入内容",
		}
	},
	data() {
		return {};
	}
}
</script>

<style lang="scss" scoped>
.search {
	padding: 20rpx 30rpx;
}

.search-container {
	height: 36px;
	padding: 0 10px;
	display: flex;
	align-items: center;
	border: 1px solid #808080;
	background-color: #FFFFFF;
	border-radius: 15px;
}

.search-image {
	width: 20px;
	height: 20px;
}

.search-placeholder {
	padding-left: 8px;
	font-size: 15px;
	color: #999999;
}
</style>
