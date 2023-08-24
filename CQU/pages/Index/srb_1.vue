<template>
	<view class="count">
		<view :animation="animationData" style="background:lightgoldenrodyellow;height:45rpx;width:45rpx">
			
		</view>
	<view class="mode1">
		<strong>根基雄厚</strong>
	</view>
	<view class="mode2">
	    重庆大学，长期以来致力于大学生德智体美劳的全面发展，
		采用最先进的科技手段，与其他学校联合建立教学新模式。学校成立几个
		月来造就了一批又一批的优秀学生。
	</view>
	<view :animation="animationData" style="background:lightgoldenrodyellow;height:45rpx;width:45rpx">
		
	</view>
	<view class="mode1">
		<strong>成绩卓越</strong>
	</view>
	<view class="mode2">
		建校以来，重庆大学累积学员近千人，学生的专业技术得到了极大的提升，在我校学习的学
		生都顺利的找到了工作，过上了998的生活。
		</view>
		<view :animation="animationData" style="background:lightgoldenrodyellow;height:45rpx;width:45rpx">
			
		</view>
		<view class="mode1">
			<strong>重庆大学的特色</strong>
		</view>
		<view class="mode2">
			1.聘请经验丰富的教师:聘请了重庆大学的老师，具有丰富的教学经验，制作了优美的PPT，
			让学生一看就懂。
			</view>
			<br>
			<view class="mode2">
			2.运用了先进的设备，人手一台笔记本电脑和电子平板。
			</view>
			<br>
			<view class="mode2">
			3.规范的教室管理模式，采用个人备课和集体备课相结合的形式，对质量严格把关
			，保证高效利用每节课
			</view>
			<br>
			<view class="mode2">
			4.因材施教：为每个学生量身打造学习方案，做到真正的因材施教。
			</view>
			<br>
			<view class="mode2">
			5.人性化的教育理念：不排斥差的学生，重视学生兴趣的培养，重视对学生学习方法
			的指导。
			</view>
			<br>
			<view class="mode2">
			6.拓展培训：不仅在于提升学生的能力，更重要的是让学生知道学习的重要性，为什么而
			学，怎么样学。提升学生的整体素质。
			</view>
			<br>
			<view class="mode2">
			7.教师的敬业精神和责任心：年轻富有活力，具有创新精神，关注学生的学习和成长。
			</view>
			<br>
			<br>
	</view>
	
</template>

<script>
	export default{
	  data() {
	    return {
	      animationData: {}
	    }
	  },
	  onShow: function(){
	    var animation = uni.createAnimation({
	      duration: 1000,
	        timingFunction: 'ease',
	    })
	
	    this.animation = animation
	
	    animation.scale(2,2).rotate(45).step()
	
	    this.animationData = animation.export()
	
	    setTimeout(function() {
	      animation.translate(30).step()
	      this.animationData = animation.export()
	    }.bind(this), 1000)
	  },
	  methods:{
	    rotateAndScale: function () {
	      // 旋转同时放大
	      this.animation.rotate(45).scale(2, 2).step()
	      this.animationData = this.animation.export()
	    },
	    rotateThenScale: function () {
	      // 先旋转后放大
	      this.animation.rotate(45).step()
	      this.animation.scale(2, 2).step()
	      this.animationData = this.animation.export()
	    },
	    rotateAndScaleThenTranslate: function () {
	      // 先旋转同时放大，然后平移
	      this.animation.rotate(45).scale(2, 2).step()
	      this.animation.translate(100, 100).step({ duration: 1000 })
	      this.animationData = this.animation.export()
	    }
	  }
	}
</script>

<style>
.mode1{
	margin-top: 35rpx;
	 margin-left: 180rpx; 
	font-size: 45rpx;
	letter-spacing: 3rpx;
	color:#000000;
	margin-bottom: 15rpx;
}
.count{
	
}
page {
	background-image: url('~@/static/jp2.jpg'); 
}
.mode2{
	font-size: 36rpx;
	margin-left: 60rpx;
	margin-right: 60rpx;
	letter-spacing: 4rpx;
	text-indent:40px;
}

</style>
