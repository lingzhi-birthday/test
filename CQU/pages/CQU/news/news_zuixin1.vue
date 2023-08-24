<template>
	<view>
		<view>
			<view class="u_map">
					<u-swiper :list="list":height="470" effect3d="true"></u-swiper>
				</view>
				<view class="tit"><strong>重庆大学2023年本科学生搬迁工作顺利结束</strong></view>
				<view class="t_1">
					按照学校总体部署和要求，重庆大学虎溪校区2023年学生宿舍搬迁工作于7月8日—7月18日顺利开展。搬迁工作分为校区间搬迁和虎溪校区内搬迁两部分，其中虎溪校区搬迁至沙坪坝校区本科生涉及15个学院165个行政班，共计4287人，虎溪校区内搬迁4500人。</view>
			
				<view class="t_2">针对本年度搬迁工作涉及人数多、调整范围广、搬迁时间分散、天气酷热等诸多因素，学校高度重视，周密部署。虎溪管委会根据学校搬迁工作领导小组的总体要求和安排，详细拟订了搬迁工作方案。 虎溪管委会、学工部、保卫处、后勤处、校医院等部门与各学院协调有序，分工明确，搬迁工作平稳有序、安全高效。
7月15日，41辆贴有统一标识的客、货车准时就位。电气学院、土木学院的同学们早已提前收拾好行李，按照“行李先装车，同学后上车”的顺序排队上车，顺利发车前往沙坪坝校区。7月17日上午，随着最后一批搬迁学生顺利到达沙坪坝校区，2023年本科学生校区间搬迁工作顺利完成。</view>
				<view class="t_3">为保障学生顺利入住，拥有一个良好的住宿环境，新大正学校事业部协调50余名一线员工参与保洁等工作，在有限的时间内以最快的速度，在搬迁工作开始前将学生宿舍打扫整理干净；校区搬迁期间，新大正学校物业党支部号召弘扬奉献精神，发挥党员先锋模范作用，组织抽调党员、干部和曾在虎溪校区工作过的员工共26名志愿者支援搬迁工作，保证搬迁工作有序、平安、顺利进行。</view>
				<view class="t_3">人性化的工作方式、平稳有序的搬迁现场、安全高效的搬迁过程获得了学生的一致好评。“本来以为搬迁会需要很多时间，但是在大家的共同努力下，我再次感受到重大速度！”2021级法学院方英伟同学骄傲地说。热火朝天的搬迁过程中也藏着同学们离别愁绪和美好祝愿，2021级经济与管理学院韩晨阳同学说到：“最不舍的就是在虎溪相识两年的朋友，再也不能经常一起踢球，一起排练。虽然我离开了虎溪，但美好的回忆将永远留在心里。”</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				list: [
					{
						image: '/static/cqu_map/900.jpg',
					},
					{
						image: '/static/cqu_map/901.jpg',
					},
					{
						image: '/static/cqu_map/902.jpg',
					}
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