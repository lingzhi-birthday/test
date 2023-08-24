<template>
	<view>
		<view>
			<view class="u_map">
					<u-swiper :list="list":height="470" effect3d="true"></u-swiper>
				</view>
				<view class="tit"><strong>重庆大学第三十一届校园歌手大赛</strong></view>
				<view class="t_1">
					2023年5月28日晚，“重庆农商行杯”重庆大学第三十一届校园歌手大赛总决赛在A区风雨操场举办，20余名优秀校园歌手、近10000名师生观众共同见证了本届校园歌手大赛冠军的诞生，以及优秀校园歌手光荣绽放的高光时刻。重庆发布以及重庆大学、重大青年等融媒体平台进行全程直播，累计吸引85万余人次线上观看。</view>
			
				<view class="t_2">重庆大学全面贯彻落实习近平总书记关于青年工作的重要思想和关于文艺工作的重要论述，多措并举满足全校师生精神文化需求，推动校地文化共建、文化育人走深走实，大力弘扬中华优秀传统文化，助力新时代新征程“百年新重大”高质量发展， 为推进中华民族伟大复兴贡献重大力量。

</view>
				
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				list: [{
						image: '/static/cqu_map/925.jpg',
					},
					{
						image: '/static/cqu_map/926.png',
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
