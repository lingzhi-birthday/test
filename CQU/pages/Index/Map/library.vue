<template>
	<view>
		<view>
			<view class="u_map">
					<u-swiper :list="list":height="470" effect3d="true"></u-swiper>
				</view>
				<view class="tit"><strong>重庆大学图书馆</strong></view>
				<view class="t_1">
					重庆大学图书馆是重庆大学的主要图书馆，位于重庆市沙坪坝区，是该校学术资源和信息服务的重要支持单位之一。图书馆建筑面积约4.6万平方米，馆内设有多个阅览室和自习室，提供舒适的学习环境。</view>
			
				<view class="t_2">为了方便读者的学习和研究，重庆大学图书馆还设有电子阅览室和多媒体学习区域，读者可以利用电脑、互联网和多媒体设备查阅电子资源、学习各类软件和工具。</view>
				<view class="t_3">总体而言，重庆大学图书馆是学校重要的学术支持机构，为师生提供图书馆资源和信息服务，促进学校的教学和科研工作。</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				list: [{
						image: '/static/cqu_map/li.jpg',
					},
					{
						image: '/static/cqu_map/li_1.jpg',
					},
					{
						image: '/static/cqu_map/li_2.jpg',
					}
				]
			}
		},
	methods: {

	}
	}
</script>

<style>
	<style lang="scss" scoped>
	.u_map1 {
		height:1000rpx;
	}
	.t_1 {
		color:gray;
		font-size: 18px;
		margin-top: 40rpx;
		margin-right: 60rpx;
		margin-left: 60rpx;
		text-indent: 21px;
		letter-spacing: 6rpx;
		margin-bottom: 10rpx;
	}
	.t_2 {
		color:gray;
		font-size: 18px;
		margin-top: 10rpx;
		margin-right: 60rpx;
		margin-left: 60rpx;
		text-indent: 21px;
		letter-spacing: 6rpx;
		margin-bottom: 10rpx;
	}
	.t_3 {
		color:gray;
		font-size: 18px;
		margin-top: 10rpx;
		margin-right: 60rpx;
		margin-left: 60rpx;
		text-indent: 21px;
		letter-spacing: 6rpx;
		margin-bottom: 10rpx;
	}

	.tit {
		margin-top: 50rpx;
		color: rgb(0, 0, 0);
		font-size: 55rpx;
		letter-spacing: 4rpx;
		text-align: center;
	}
	page{
		background-image: url('/static/cqu_map/back7.png');
	}
</style>