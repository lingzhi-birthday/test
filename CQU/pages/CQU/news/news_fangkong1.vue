<template>
	<view>
		<view>
			<view class="u_map">
					<u-swiper :list="list":height="470" effect3d="true"></u-swiper>
				</view>
				<view class="tit"><strong>关于A、B校区实施封闭管理的通知</strong></view>
				<view class="t_1">
					月23日重庆市沙坪坝区新型冠状病毒肺炎疫情防控指挥部发布关于新增疫情风险区域的通告，我校A校区学生五公寓、B校区管理科学与工程学院大楼划定为高风险区，A、B校区范围内高风险区以外的区域划定为中风险区。为切实有效做好我校疫情处置和防控工作，经学校疫情防控工作领导小组研究，决定对A、B校区实施封闭管理。</view>
			
				
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				list: [{
						image: '/static/cqu_map/929.jpg',
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