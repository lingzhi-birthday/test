<template>
	<view>
		<image class="u_map" src="/static/CQU/CQU_map.jpg">
		<view class="u-m-t-20 u-p-0">
			<u-cell-group>
				<u-cell-item icon="play-right-fill" title="图书馆" @click="goToli"></u-cell-item>
				<u-cell-item icon="play-right-fill" title="第一教学楼" @click="goToD1"></u-cell-item>
				<u-cell-item icon="play-right-fill" title="第一实验楼" @click="goToDS1"></u-cell-item>
				<u-cell-item icon="play-right-fill" title="缙湖云湖" @click="goToJHYH"></u-cell-item>
				<u-cell-item icon="play-right-fill" title="风雨操场" @click="goTofengyu"></u-cell-item>
				</u-cell-group>
			</u-cell-group>
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
			
			getposition(event){
				var x=event.touches[0].clientX
				var y=event.touches[0].clientY
				console.log(x)
				console.log(y)
				  if(99<x&&x<145&&229<y&&y<246){
					  uni.navigateTo({
					  	url:"beimen"
					  })
				  }else if(83<x&&x<109&&42<y&&y<70){uni.navigateTo({
					  	url:"library"
					  })}else if(69<x&&x<106&&87<y&&y<114){uni.navigateTo({
					  	url:"yunhu"
					  })}else if(126<x&&x<158&&126<y&&y<156){uni.navigateTo({
					  	url:"zonghelou"
					  })}else if(68<x&&x<105&&127<y&&y<159){uni.navigateTo({
					  	url:"D1"
					  })}else if(25<x&&x<61&&125<y&&y<162){uni.navigateTo({
					  	url:"DS1"
					  })}else if(46<x&&x<75&&41<y&&y<71){uni.navigateTo({
					  	url:"yishulou"
					  })}else if(165<x&&x<204&&10<y&&y<38){uni.navigateTo({
					  	url:"lanyuan"
					  })}else if(157<x&&x<180&&50<y&&y<69){uni.navigateTo({
					  	url:"huodongzhongxin"
					  })}
			},
			goToli() {
				uni.navigateTo({
					url: "/pages/Index/Map/library"
				})
			},
			goToDS1() {
				uni.navigateTo({
					url: "/pages/Index/Map/DS1"
				})
			},
			goToD1() {
				uni.navigateTo({
					url: "/pages/Index/Map/D1"
				})
			},
			goToJHYH() {
				uni.navigateTo({
					url: "/pages/Index/Map/JHYH"
				})
			},
			goTofengyu() {
				uni.navigateTo({
					url: "/pages/Index/Map/fengyu"
				})
			},
		}
	}
</script>

<style>
/* 	.container{
		positiom:relative;
	}
	.top{
		position:absolute;
		z-index:1;
	}
	.bottom{
		position:absolute;
		z-index:0;
	} */
	
	.u_map{
	  width:380px;
	  height:260px;
	  vertical-align: middle;
	  display: table-cell;
	  text-align: center;
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
		
	page{
		background-image: url('/static/cqu_map/back4.png');
	}
</style>
