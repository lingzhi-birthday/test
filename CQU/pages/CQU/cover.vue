<template>
	<view>
		<br>
		
		<view class="mode">
			
		</view>
		<image class="logo" src="../../static/CQU.png">
		</image>
		<view class="mode2">
			重大校训
		</view>
		<view class="mode3">
			耐劳苦，尚俭朴，勤学业，爱国家
		</view>
		
		<view class="mode3">
			研究学术、造就人才、佑启乡邦、振导社会
		</view>
		<view class="index" @click="gotoindex">
			点击进入重庆大学首页
		</view>
		<view class="in">
			(点击进入)
		</view>
	</view>
	
</template>

<script>
	export default {
		methods:{
			gotoindex(){
				 wx.switchTab({
					url:"../../pages/index/index"				,
					})
			},
		}
		
	
	}
</script>

<style>
	.mode{
		margin-top: 50px;
		text-align: center;
		font-size: 40rpx;
		color: green;
	}
	
	.mode2 {
		margin-top: 40px;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		color: black;
		font-size: 50rpx;
	}

	.logo {
		height: 400rpx;
		width: 400rpx;
		margin-top: 150rpx;
		left: 23%;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: auto;
	}

	.mode3 {
		margin-top: 15px;
		font-size: 40rpx;
		text-align: center;
		color: #8f8f94;
	}
	.top {
		font-size: 40rpx;
		color: #55aaff;
	}

	.title {
		
		font-size: 36rpx;
		color: #8f8f94;
	}
	.bottom{
		margin-top: 580rpx;
		font-size: 55rpx;
		color: #ff 0000;
	}
	.index{
		margin-top: 200px;
		font-size: 30px;
		color: #000;;
		text-align: center;
	}
	.in{
		margin-top: ;
		text-align: center;
		font-size:40rpx ;
		color:#000;
		
	}
	page{
		 background-image:url('~@/static/cover.png');
	}
</style>
