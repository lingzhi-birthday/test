<template>
	<view>
		<view>
			<view class="u_map">
					<u-swiper :list="list":height="470" effect3d="true"></u-swiper>
				</view>
				<view class="tit"><strong>虎溪校区开展交通安全宣传教育活动</strong></view>
				<view class="t_1">
					为深入贯彻落实习近平总书记关于安全生产重要论述和党的二十大精神，持续树牢安全红线意识，推动校园安全责任落实，进一步提高师生员工安全意识和避险逃生能力，6月16日，虎溪校区组织开展了消防应急演练和道路交通事故综合应急演练活动，同时开展了“6.16安全宣传咨询日” 活动。 </view>
			
				<view class="t_2">活动针对校际车队和校内电瓶车队驾驶员及管理人员进行，内容包括海姆立克急救、安全用电、火灾逃生等，具体学习了灭火器、防毒面具、灭火毯等消防器材的正确使用方法。在全面掌握应急处置及逃生方法后，开展了应急处置演练。通过模拟大客车追尾引发车辆起火燃烧事故现场，围绕人员疏散、伤员急救、明火扑灭等方面开展应急演练。演练结束后，工作人员向师生发放《安全宣传五进手册》《应急安全知识手册》，并进行一年一度的 “6.16安全宣传咨询日”活动。</view>
				<view class="t_3">本次活动通过专业培训和实地演练，增强了驾驶人员以及师生员工的安全意识，提高了应急处置和逃生能力，营造了“人人讲安全，个个会应急”的安全知识学习氛围。</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				list: [{
						image: '/static/cqu_map/906.jpg',
					},
					{
						image: '/static/cqu_map/907.jpg',
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