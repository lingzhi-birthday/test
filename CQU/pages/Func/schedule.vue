<template>
	<view class="image">
		<view class="header">
	       <image src="/static/Xiaoche/shikebiao_head.png"style="height: 200px;"></image>
	    </view>
	    <view class="content"style="margin-top: 100px;">
	         <image src="/static/Xiaoche/shikebiao1.png"style="margin-left: 50px;"></image>
	         <image src="/static/Xiaoche/shikebiao2.png"style="margin-left: 50px;"></image>
	    </view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		}
	}
</script>

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
     width: 750rpx;
     height: 200rpx;
     background: rgba(63, 205, 235, 1);
     box-shadow:rgba(63, 205, 235, 0.47);
     margin-top: 30rpx;
     margin-left: auto;
     margin-right: auto;
   }
   
   .header image {
     width: 750rpx;
     height: 200rpx;
    
   }
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
	.content{
		width:750rpx;
		height:500rpx;
	}
  
</style>
