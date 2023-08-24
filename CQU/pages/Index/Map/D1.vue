<template>
	<view>
		<view class="tit"><strong>第一教学楼</strong></view>
		<view class="t_2">重庆大学虎溪校区的第一教学楼是该校主要的教学建筑之一，它位于校园的中心位置，是学校师生们学习和交流的重要场所之一。</view>
		<view class="t_1">第一教学楼是一座现代化的建筑，采用了现代风格设计。它的外立面通常采用玻璃幕墙和混凝土结构，给人一种简洁而富有现代感的印象</view>
		<image class="u_map1" src="../../../static/cqu_map/D1_2.png">
		<view class="t_1">第一教学楼内设有多个教室，包括大型讲堂和普通教室。这些教室配备了先进的多媒体设备，如投影仪、电子白板和音响系统，以提供良好的教学环境。</view>
		<view class="t_1">教学楼还设有教师办公室和研究室，供教师和研究人员使用。这些办公室提供了一个良好的工作环境，有助于教师们进行教学和研究工作。</view>
		<image class="u_map3" src="../../../static/cqu_map/D1_2.jpg">
		<view class="t_1">在第一教学楼内，学生们可以使用丰富的学习资源。楼内提供了图书馆和自习室，学生可以在这里阅读图书、借阅资料并进行自主学习。除了教室和办公室，第一教学楼还提供了一些社交空间，如休息区和茶水间。这些空间为师生们提供了一个放松和交流的场所，促进了师生之间的互动和合作。</view>
		<image class="u_map2" src="../../../static/cqu_map/D1_1.jpg">
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
	.u_map1{
	  
	  width:300px;
	  height:150px;
	  left: 10%;
	  margin-top: 30rpx;
	  margin-bottom: 30rpx;
	}
	.u_map3{
	  
	  width:300px;
	  height:180px;
	  left: 10%;
	  margin-top: 30rpx;
	  margin-bottom: 30rpx;
	}
	.u_map2{
	  
	  width:300px;
	  height:150px;
	  left: 10%;
	  margin-top: 30rpx;
	  margin-bottom: 30rpx;
	}
	.t_1 {
		
		color:gray;
		font-size: 15px;
		margin-top: 10rpx;
		margin-right: 60rpx;
		margin-left: 60rpx;
		text-indent: 21px;
		letter-spacing: 6rpx;
		margin-bottom: 10rpx;
	}
	.t_2 {
		
		color:gray;
		font-size: 15px;
		margin-top: 10rpx;
		margin-right: 60rpx;
		margin-left: 60rpx;
		text-indent: 21px;
		letter-spacing: 6rpx;
		margin-bottom: 10rpx;
	}
	.tit {
		margin-top: 40rpx;
		margin-bottom: 30rpx;
		color: rgb(0, 0, 0);
		font-size: 45rpx;
		letter-spacing: 4rpx;
		text-align: center;
	}
	page{
		background-image: url('/static/cqu_map/back5.png');
	}
</style>