<template>
   <view class="image">
	   
	<view class="header">
		<text> 重庆大学2023-2024学年校历</text>
    </view>
	
	<view class="calendar1">
		<image src="/static/Xiaoli/calendar_achieve.png"style="margin-left: 25px;"></image>
	</view>
	
	<view class="calendar2">
		<image src="/static/Xiaoli/calendar_achieve1.png"style="margin-left: 25px;"></image>
	</view>
   </view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		}
	}
</script>

<style>
    .header {
      width: 400rpx;
      height: 80rpx;
      margin-top: 30rpx;
      margin-left: auto;
      margin-right: auto;
    }
	
	.calendar1{
	width:800rpx;
	height: 150rpx;
	
	border-radius: 20%;
	margin-top: 20rpx;
	margin-left: auto;
	margin-right: auto;}
	
	.calendar2{
	width: 800rpx;
	height: 150rpx;
	
	border-radius: 20%;
	margin-top: 350rpx;
	margin-left: auto;
	margin-right: auto;}
	
	.image {
	        will-change: transform;
	        width: auto;
	        height: auto;
	        image-rendering:-moz-crisp-edges;
	        image-rendering:-o-crisp-edges;
	        image-rendering:-webkit-optimize-contrast;
	        image-rendering: crisp-edges;
	        -ms-interpolation-mode:nearest-neighbor;
	    }
</style>
