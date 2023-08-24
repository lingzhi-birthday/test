<template>
	<view>
		<view>
			<view class="u_map">
					<u-swiper :list="list":height="470" effect3d="true"></u-swiper>
				</view>
				<view class="tit"><strong>虎溪分工会开展“‘粽’夏好时光 你我共端阳”端午节主题活动</strong></view>
				<view class="t_1">
					浓浓粽叶香，暖暖端午情。为丰富教职工文化生活，弘扬传统民俗文化，6月15日，虎溪分工会开展了“‘粽’夏好时光 你我共端阳”端午节主题活动，分工会70余人参加。</view>
			
				<view class="t_2">除此之外，活动特地安排了我国非遗技艺“植物拓染”，让大家在DIY过程中感受自然之美。拓染开始前，需要用明矾加清水对植物花叶进行浸泡，以保证固色效果。在经过选材、配色、造型、固定、敲击等环节后，一幅幅造型美观、纹理清晰、色彩艳丽的“植物画”便呈现在了白色帆布袋上，植物中的青草香也一并被保留下来。</view>
				<view class="t_3">本次活动不仅让教职工深刻体会了中国传统节日的文化内涵，也以轻松愉快的方式锻炼了大家的动手能力和学习能力，最后为大家提供了互相了解交流的机会，增强了单位的凝聚力和向心力。</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				list: [{
						image: '/static/cqu_map/921.jpg',
					},
					{
						image: '/static/cqu_map/920.jpg',
					},
					{
						image: '/static/cqu_map/919.jpg',
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