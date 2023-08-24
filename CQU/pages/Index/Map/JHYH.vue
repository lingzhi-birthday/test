<template>
	<view>
		<view>
			<view class="u_map">
					<u-swiper :list="list":height="470" effect3d="true"></u-swiper>
				</view>
				<view class="tit"><strong>缙湖云湖</strong></view>
				<view class="t_1">
					老门柱广场身后便是云湖。缙湖和云湖之名均源自校区紧邻的缙云山，取“湖映山，山水相依相融”之意。缙湖、云湖的规划始终秉持着原生态与人文校园建设相和谐的理念，采取顺势而为的园林布局，体现出满含人文关怀背景下的自然风情。</view>
			
				<view class="t_2">微风轻拂 荷花摇曳两侧湖水波光潋滟 交相辉映层层鳞浪随风而起 美不胜收但在驻足赏景时千万别忘欣赏</view>
				
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				list: [{
						image: '/static/cqu_map/860.jpg',
					},
					{
						image: '/static/cqu_map/861.jpg',
					},
					{
						image: '/static/cqu_map/862.jpg',
					},
					{
						image: '/static/cqu_map/863.jpg',
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