<template>
	<view>
		<view>
			<view class="u_map">
					<u-swiper :list="list":height="470" effect3d="true"></u-swiper>
				</view>
				<view class="tit"><strong>虎溪校区举办食堂餐品品鉴交流会</strong></view>
				<view class="t_1">
					为进一步落实食品安全责任，满足师生餐饮需求，6月1日，虎溪三食堂举办了餐品品鉴交流会，并现场收集了师生意见和建议。</view>
			
				<view class="t_2">此次品鉴交流会邀请了60多名师生，提供了40余道餐品（其中新品20余个）供师生品鉴。现场装饰精美的长桌、整齐摆放的餐具、丰富多样的菜品，让品鉴过程更加的轻松愉快。</view>
				<view class="t_3">秉承“为师生提供优质餐饮服务”的宗旨，虎溪校区食堂每年都会开展餐品品鉴交流会，邀请部分师生参与部分餐品品鉴和新品试吃，食堂将根据反馈的意见和建议进行相应调整，更好地改进菜品品质，提升服务质量，提高师生满意度。</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				list: [{
						image: '/static/cqu_map/922.png',
					},
					{
						image: '/static/cqu_map/920.jpg',
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