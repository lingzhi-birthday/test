<template>
	<view content="content">
		  <view class="header">
		    <image src="/static/CQU.jpeg"></image>
		  </view>
		
		
		<u-grid :col="2" style="margin-top: 10px;">
			<br>
				<u-grid-item>
					<u-icon label="" size="60" name="/static/icon/pay/yue.png">
						
					</u-icon>
					<view class="gg" @click="gotoyue()">余额</view>
				</u-grid-item>
				<u-grid-item>
					<u-icon label="" size="60" name="/static/icon/pay/zhangdan.png">
						
					</u-icon>
					<view class="gg" @click="gotozhangdan()">账单查询</view>
				</u-grid-item>
				<u-grid-item>
					<u-icon label="" size="60" name="/static/icon/pay/chongzhi.png">
						
					</u-icon>
					<view class="gg" @click="gotochongzhi()">充值</view>
				</u-grid-item>
				<u-grid-item>
					<u-icon label="" size="60" name="/static/icon/pay/jiaofei.png">
						
					</u-icon>
					<view class="gg" @click="gotosjiaofei()">缴费</view>
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
			gotoyue(){
				uni.navigateTo({
					url:"/pages/Func/bank/yue"
				})
				
			},
			gotozhangdan(){
				uni.navigateTo({
					url:"/pages/Func/bank/zhangdan"
				})
				
			},
			gotochongzhi(){
				uni.navigateTo({
					url:"/pages/Func/bank/chongzhi"
				})
				
			},
			gotosjiaofei(){
				uni.navigateTo({
					url:"/pages/Func/bank/jiaofei"
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
