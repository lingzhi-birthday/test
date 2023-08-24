<template>
	<view content="content">
		  <view class="header">
		    <image src="/static/CQU.jpeg"></image>
		  </view>
		
		
		<u-grid :col="2">
			<br>
				<u-grid-item>
					<u-icon label="" size="35" name="/static/icon/func/calendar.png">
						
					</u-icon>
					<view class="gg" @click="gotocalendar">校历</view>
				</u-grid-item>
				
				<u-grid-item>
					<u-icon label="" size="35" name="/static/icon/func/library.png">
						
					</u-icon >
					<view class="gg" @click="gotolibrary">图书馆占位</view>
				</u-grid-item>
				
				<u-grid-item>
					<u-icon label="" size="35" name="/static/icon/func/pay.png">
						
					</u-icon>
					<view class="gg" @click="gotopay">财小通</view>
				</u-grid-item>
				
				<u-grid-item>
					<u-icon label="" size="35" name="/static/icon/func/schedule.png">
						
					</u-icon>
					<view class="gg" @click="gotoschedule">校车时刻表</view>
				</u-grid-item>
				<u-grid-item>
					<u-icon label="" size="35" name="/static/icon/func/activity.png">
						
					</u-icon>
					<view class="gg" @click="gotoactivity">校园活动</view>
				</u-grid-item>
			</u-grid>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			gotocalendar(){
				uni.navigateTo({
					url:"/pages/Func/calendar"
				})
				
			},
			gotolibrary(){
				uni.navigateTo({
					url:"/pages/Func/library"
				})
				
			},
			gotopay(){
				uni.navigateTo({
					url:"/pages/Func/pay"
				})
				
			},
			gotoschedule(){
				uni.navigateTo({
					url:"/pages/Func/schedule"
				})
				
			},
			
			gotoactivity(){
				uni.navigateTo({
					url:"../../pages/func/activity"
				})
				
			}
			
			
			
		}
	}
</script>

<style>
 .header image {
    width: 161rpx;
    height: 161rpx;
    border-radius: 50%;
  }
  .header {
    width: 161rpx;
    height: 161rpx;
    background: rgba(63, 205, 235, 1);
    box-shadow: 0rpx 12rpx 13rpx 0rpx rgba(63, 205, 235, 0.47);
    border-radius: 50%;
    margin-top: 30rpx;
    margin-left: auto;
    margin-right: auto;
  }
  .content {
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
</style>
