<template>
	<view>
		<view>
			<view class="u_map">
					<u-swiper :list="list":height="470" effect3d="true"></u-swiper>
				</view>
				<view class="tit"><strong>计算机学院VS体育学院</strong></view>
				<view class="t_1">
					 谁是那匹更黑的马？两支球队都是首次进入四强，计算机学院本届比赛低开高走，首场比赛大比分负于土木学院，第二场上半场又处于落后的情势下，绝境之处爆发惊人的战力，先是逆转机械，后又力克材料，站上了半决赛的赛场。对计算机学院而言，板凳深度不足是其最大的劣势，能否在半决赛中克服前面三场球略有透支的体能，将是他们能否逆风翱翔，冲进决赛的胜负手！</view>
			
				<view class="t_2">体育学院虽然没有足球项目的高水平球员，但是平均身体力量水平处于断档领先，暴力身体流的冲击型踢法很容易让对手在节奏上不适应，在比赛中能否把身体力量的优势转化为比分上的胜势，将是体育学院能否站上决赛赛场的关键！</view>
				
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				list: [{
						image: '/static/cqu_map/910.jpg',
					},
					{
						image: '/static/cqu_map/911.jpg',
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