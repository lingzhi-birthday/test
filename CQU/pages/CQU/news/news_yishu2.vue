<template>
	<view>
		<view>
			<view class="u_map">
					<u-swiper :list="list":height="470" effect3d="true"></u-swiper>
				</view>
				<view class="tit"><strong>“即兴青春”草坪音乐节</strong></view>
				<view class="t_1">
					2023年5月27日，由教育部高校思想政治工作创新发展中心（重庆大学）主办，重庆大学党委宣传部、校团委、虎溪校区党工委、虎溪校区管委会承办的“即兴青春”2023草坪音乐节在重庆大学虎溪校区东门草坪举办。</view>
			
				<view class="t_2">为随着《知足》《是妈妈是女儿》《陪你度过漫长岁月》等40首歌曲近4小时的尽情演绎，一场安全、尽兴，富有青春活力的文艺活动随之落下帷幕。</view>
				
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				list: [{
						image: '/static/cqu_map/927.jpeg',
					},
					{
						image: '/static/cqu_map/928.jpeg',
					},
					{
						image: '/static/cqu_map/li_2.jpg',
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