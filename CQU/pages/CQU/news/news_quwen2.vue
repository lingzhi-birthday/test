<template>
	<view>
		<view>
			<view class="u_map">
					<u-swiper :list="list":height="470" effect3d="true"></u-swiper>
				</view>
				<view class="tit"><strong>《丹青漫行—重庆大学艺术学院学生中国画6人展》画展在虎溪校区开幕</strong></view>
				<view class="t_1">
					4月6日下午，《丹青漫行—重庆大学艺术学院学生中国画6人展》在重庆大学虎溪校区人文艺术展厅开幕。重庆大学艺术学院院长、美育教育中心主任雒三桂，艺术学院副院长张楠木，党委宣传部副部长徐方正，学生代表等出席开幕式，开幕式由虎溪管委会办公室主任姜林主持。</view>
			
				<view class="t_2">此次画展是虎溪校区开展的系列文化活动之一，为师生提供了一个展示、交流、创作的平台，有利于加强新时代学校美育工作开展和校园文化建设。据悉，此次画展将持续到4月28日，欢迎各位师生前往观展。</view>
				
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				list: [{
						image: '/static/cqu_map/924.jpg',
					},
					{
						image: '/static/cqu_map/919.jpg',
					},
					
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