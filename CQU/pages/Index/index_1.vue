<template>
	<view >
		
		<u-swiper class="info":height="420":list="list1":title="title1" effect3d="true">
		</u-swiper>
		<view class="info_1">
		<view class="u-m-t-20">
			<view class="title2">
				
				最新公告
				
			</view>
			<u-cell-group>
				<br>
				<u-cell-item  @click='gotosrb' title="2022-5-7 招生简章"></u-cell-item>
				<br>
				<!-- <u-cell-item icon="photo" title="相册"></u-cell-item> -->
				<u-cell-item  @click='gotorps' title="2022-7-9 报道流程"></u-cell-item>
				<!-- <u-cell-item icon="heart" title="关注"></u-cell-item> -->
			</u-cell-group>
			<br>
			<view class="title2">
				
				热点查询
				
			</view>
			<u-grid :col="2">
				<br>
					<u-grid-item>
						
						<view class="gg" @click="gotocount">学校招收总人数</view>
					</u-grid-item>
					<u-grid-item>
						
						<view class="gg" @click="gotomap">校园地图</view>
					</u-grid-item>
				</u-grid>
				<br>
				<view class="title2">
					
					专家谈专业
					
				</view>
					
				<u-swipe-action  :index="index"
					v-for="(item, index) in list2" :key="item.id" 
				>
					<view class="item u-border-bottom">
						<image mode="aspectFill" :src="item.images" />
						
						<view class="title-wrap">
							<text class="title11">{{ item.title }}</text>
						</view>
					</view>
				</u-swipe-action>
				
				<view class="title2">
					<br>
					专业介绍
					
				</view>
					
				<u-line color="blue" />
					<view class="mode1"@click="gotoCST">
						
						计算机科学与技术
					</view>
					
					<u-line color="blue" />
						<view class="mode1"@click="gotoITE">
						
							物联网工程
						</view>
						
						<u-line color="blue" />
							<view class="mode1"@click="gotoisy">
								
								信息安全
							</view>
							
							<u-line color="blue" />
								<view class="mode1"@click="gotoEEy">
									
									工程与能源
								</view>
								
								<u-line color="blue" />
									<view class="mode1"@click="gotoeeg">
										
										电气工程
									</view>
									
					<u-line color="blue"></u-line>
					</view>
		</view>
	</view>   

</template>

<script>
	export default {
		data() {
			return {
				list1: [{
						image: '/static/lunbo/index/yunhu.jpg',
						title: '研究学术'
					},
					{
						image: '/static/lunbo/index/yijiao.jpg',
						title: '造就人才'
					},
					{
						image: '/static/lunbo/index/beimen.jpg',
						title: '佑启乡邦'
					},
					{
						image: '/static/lunbo/index/tiyuzhongxin.jpg',
						title: '振导社会'
					}
					
				],
				title1:true,
				list2: [
					{
						id: 1,
						title: '计算机科学讲座：正在介绍专业知识',
						images: '../../static/zy1.webp',
						
					},
					{
						id: 2,
						title: '工程与能源专业专家讲解培养方案',
						images: '../../static/zj2.webp',
						
					},
					{
						id: 3,
						title: '电气工程专家在介绍专业的前景',
						images: '../../static/zj3.webp',
						
					}
				],
				disabled: false,
				btnWidth: 180,
				show: false,
				
			}
		},
		methods: {
			gotosrb(){
				uni.navigateTo({
					url:"/pages/Index/srb"				,
					})
			},
			gotorps(){
				uni.navigateTo({
					url:"/pages/Index/rps"
				})
			},
			gotocount(){
				uni.navigateTo({
					url:"/pages/Index/CQUcount"
				})
			},
			gotomap(){
				uni.navigateTo({
					url:"/pages/Index/Map/map"
				})
			},
			gotoITE(){
				uni.navigateTo({
					url:"/pages/Index/Major/ITE"
				})
			},
			gotoCST(){
				uni.navigateTo({
					url:"/pages/Index/Major/CST"
				})
			},
			gotoeeg(){
				uni.navigateTo({
					url:"/pages/Index/Major/EEG"
				})
			},
			gotoEEy(){
				uni.navigateTo({
					url:"/pages/Index/Major/EEY"
				})
			},
			gotoisy(){
				uni.navigateTo({
					url:"/pages/Index/Major/ISY"
				})
			},

		}
	}
</script>

<style lang="scss" scoped>
	
	 .info_1 {
		 margin-top: 0rpx;
		padding: 60rpx;
	} 
	
	.item {
		display: flex;
		padding: 20rpx;
	}
	
	image {
		width: 120rpx;
		flex: 0 0 120rpx;
		height: 120rpx;
		margin-right: 20rpx;
		border-radius: 12rpx;
	}
	
	.title {
		text-align: left;
		font-size: 28rpx;
		color: $u-content-color;
		}
	.mode1{
		margin-top: 15px;
		margin-bottom: 15px;
		font-size:35rpx;
		color:gray;
		letter-spacing: 6rpx;
	}
	.title2{
		font-size: 25px;
		margin-bottom: 10rpx;
	}
	.title11{
		letter-spacing: 6rpx;
	}
	.gg{
		font-size: 29rpx;
	}
	page{
		background-image: url('/static/cqu_map/back6.png');
	}
</style>