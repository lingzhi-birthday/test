<template>
	<u-time-line>
		<u-time-line-item nodeTop="2">
			<!-- 此处自定义了左边内容，用一个图标替代 -->
			<template v-slot:node>
				<view class="u-node" style="background: #19be6b;">
					<!-- 此处为uView的icon组件 -->
					<u-icon name="pushpin-fill" color="#fff" :size="24"></u-icon>
				</view>
			</template>
			<template v-slot:content>
				<view>
					<view class="u-order-title">报道流程</view>
					<view class="u-order-desc">1.入学前根据新生报到手册里的步骤，在网上服务大厅提前缴纳学费，若未缴纳学费，从操场（下图1处）下车后请先到在软件学院前面（下图5处）缴纳相应学费。</view>
					<br>
					<image class="logo" src='../../static//CQU/CQU_1.jpg'>
				</view>
			</template>
		</u-time-line-item>
		<u-time-line-item>
			<!-- 此处没有自定义左边的内容，会默认显示一个点 -->
			<template v-slot:content>
				<view>
					<view class="u-order-desc">2.到校后根据你的专业以及所在班级知晓自己班情况，在外语学院和艺术学院（下图4，6处）找到班级窗口所在地，进行报到注册，注册时应带好自己的身份证，录取通知书以及档案袋等物件，完成后会得到校园卡，校园卡等同于饭卡，请新生妥善保管。</view>
					<image class="logo" src='../../static//CQU/CQU_2.jpg'>
				</view>
			</template>
		</u-time-line-item>
		<u-time-line-item>
			<!-- 此处没有自定义左边的内容，会默认显示一个点 -->
			<template v-slot:content>
				<view>
					<view class="u-order-desc">3.报到注册后前可往新生所在宿舍（下图7处），将自己的校园卡和身份证出示给宿舍楼下相关负责阿姨看，阿姨会告诉你你所在的宿舍，并且将宿舍钥匙交到你手上，注意宿舍楼下有相关学长等推荐校园网卡等物件，切勿轻易相信，请前往梅园六栋楼下找到相关营业厅进行办理</view>
					<image class="logo" src='../../static//CQU/CQU_3.jpg'>
				</view>
			</template>
		</u-time-line-item>
		<u-time-line-item>
			<!-- 此处没有自定义左边的内容，会默认显示一个点 -->
			<template v-slot:content>
				<view>
					<view class="u-order-desc">4.完成上述操做后应前往一食堂南广场（下图2处）拿去军训所需物资，有床垫，被子，枕头，军训服装，杯子。若还需其他日用品可在梅园三栋下方超市购买，若需要相关药物可去学校校医院（下图3处）进行购买</view>
					<image class="logo" src='../../static/CQU/CQU_4.jpg'>
				</view>
			</template>
		</u-time-line-item>
	</u-time-line>
</template>

<style lang="scss" scoped>
	.u-node {
		width: 44rpx;
		height: 44rpx;
		border-radius: 100rpx;
		display: flex;
		justify-content: center;
		align-items: center;
		background: #d0d0d0;
	}
	
	.u-order-title {
		color: #55aaff;
		font-weight: bold;
		font-size: 62rpx;
		margin-bottom: 30rpx;
	}
	
	.u-order-desc {
		color:dimgray;
		font-size: 15px;
		margin-top: 10rpx;
		margin-right: 20rpx;
		margin-left: 20rpx;
		text-indent: 21px;
		letter-spacing: 6rpx;
		margin-bottom: 10rpx;
	}
	
</style>
