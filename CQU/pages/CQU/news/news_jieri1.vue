<template>
	<view>
		<view>
			<view class="u_map">
					<u-swiper :list="list":height="470" effect3d="true"></u-swiper>
				</view>
				<view class="tit"><strong>六月毕业季</strong></view>
				<view class="t_1">
					时光荏苒，两年/四年弹指一挥间，又有一批CQUer即将离开美丽的虎溪校园，开启一段崭新的征程。你对虎溪的初印象如何，与虎溪又有着什么样的精彩故事，即将离开虎溪的你是否百感交集？下面，请跟随小天的步伐，进入虎溪十二时辰，定格专属于你的虎溪记忆吧！</view>
			
				<view class="t_2">你对虎溪的初印象如何，与虎溪又有着什么样的精彩故事，即将离开虎溪的你是否百感交集？</view>
				
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				list: [{
						image: '/static/cqu_map/916.jpg',
					},
					{
						image: '/static/cqu_map/917.jpg',
					},
					{
						image: '/static/cqu_map/918.jpg',
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