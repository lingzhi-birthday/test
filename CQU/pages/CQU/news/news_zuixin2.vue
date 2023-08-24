<template>
	<view>
		<view>
			<view class="u_map">
					<u-swiper :list="list":height="470" effect3d="true"></u-swiper>
				</view>
				<view class="tit"><strong>校领导带队到虎溪校区开展校园安全检查</strong></view>
				<view class="t_1">
					为深入贯彻落实习近平总书记关于安全生产重要论述和党的二十大精神，持续树牢安全红线意识，6月30日，副校长杨俊带队到虎溪校区开展校园安全隐患专项检查，虎溪党工委书记吴丙山、保卫处副处长崔晓奎、虎溪管委会后勤办主任陈欣陪同检查。</view>
			
				<view class="t_2">杨俊带队就松园6栋架空层电动车停放、西二门建渣中转站清理、博士生公寓附近自然演替区消防等安全隐患进行了重点检查和现场督办。在实地走访和听取相关工作人员的汇报后，杨俊要求在综合考虑安全因素和学生需求的情况下，多措施规范电动车停放；在详细了解建渣中转站的实际情况后，杨俊要求对突出隐患即查即改，从根本上消除隐患；针对博士生公寓附近自然演替区消防隐患问题，杨俊要求相关部门仔细研判、详细论证，做好整改方案。</view>
				<view class="t_3">最后，杨俊强调相关部门要深入开展校园安全隐患排查，落实落细整改措施，切实维护师生生命安全和校园安全稳定。</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				list: [{
						image: '/static/cqu_map/904.jpg',
					},
					{
						image: '/static/cqu_map/905.jpg',
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