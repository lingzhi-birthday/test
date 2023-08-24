<template>
	<view>
		<view>
			<view class="u_map">
					<u-swiper :list="list":height="470" effect3d="true"></u-swiper>
				</view>
				<view class="tit"><strong>重庆大学风雨操场</strong></view>
				<view class="t_1">
					风雨操场位于重庆大学虎溪校区的中心位置，毗邻学校的教学楼、图书馆和学生宿舍区，交通便利。</view>
			
				<view class="t_2">风雨操场占地面积较大，拥有一片平坦的草坪区域，适合进行各类户外体育活动，如跑步、足球、篮球、排球等。操场周围配备有跑道、篮球场、足球场等运动设施，设施完善。风雨操场作为学校的主要运动场地，常常举办各类体育赛事和活动。其中包括学校的运动会、校园篮球赛、足球赛等，为师生们提供了展示体育才华和参与团队活动的机会。</view>
				<view class="t_3">风雨操场是学生们进行健身锻炼的主要场所之一，每天都可以看到许多学生在这里跑步、做拉伸、进行球类运动等。操场周边也设有健身器材和休闲区，供学生们使用。</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				list: [{
						image: '/static/cqu_map/865.jpg',
					},
					{
						image: '/static/cqu_map/866.jpg',
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