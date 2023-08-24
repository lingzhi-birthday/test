<template>
	<view>
		<view>
			<view class="u_map">
					<u-swiper :list="list":height="470" effect3d="true"></u-swiper>
				</view>
				<view class="tit"><strong>虎溪党工委管委会教工二支部、三支部联合观看电影《望道》</strong></view>
				<view class="t_1">
					心有所信，方能行远，为深入学习贯彻习近平新时代中国特色社会主义思想，传承红色基因， 6月2日下午，虎溪党工委管委会教工二支部、三支部联合组织观看了复旦大学发起推动、上海电影（集团）有限公司出品的电影《望道》，以发挥电影思政育人作用，培育“宣言精神”忠实传人。</view>
			
				<view class="t_2">党员同志被革命先辈事迹深深触动，理想信念再次接受了一次深刻洗礼。二支部洪为文同志感叹道：“通过对那个时代热血青年的共情，我会更加珍惜当下幸福的生活，牢记入党初心，立足本职工作，身体力行，为实现中国式现代化贡献自己的一份微薄力量”；王苾力同志说：“敌人不会了解，‘陈望道’、‘杨阿龙’不是个人，而是一种精神，一种信仰。我诚感今日盛世来之不易，也更加坚定了听党话，跟党走的信念，立足本职工作，身体力行，致敬《望道》，致敬无数先辈们！”；三支部吴毅说：“千百万革命烈士的牺牲换来了新中国, 人民群众当家作主的国家。这也让我们更加坚信，只要我们不忘初心，不断的奋斗和努力，为社会主义事业做出更大的贡献，就一定能实现梦想”。</view>
				
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				list: [{
						image: '/static/cqu_map/908.jpg',
					},
					{
						image: '/static/cqu_map/909.png',
					},
					
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