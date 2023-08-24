<template>
	<view class="wrap">
		<u-form :model="user" ref="uForm">
			<u-form-item class="u-p-l-40" label-width="140" label-position="left" label="学号" prop="stuId">
				<u-input :border="border" placeholder="请输入学号" v-model="user.stuId"type="text"></u-input>
			</u-form-item>
			<!-- <u-form-item class="u-p-l-40" label-width="140" label-position="left" label="姓名" prop="stuName">
				<u-input :border="border" placeholder="请输入姓名" v-model="user.stuName" type="text"></u-input>
			</u-form-item> -->
			<u-form-item class="u-p-l-40" label-width="140" label-position="left" label="性别" prop="stuSex">
				<u-input :border="border" placeholder="请输入性别" v-model="user.stuSex" type="text"></u-input>
			</u-form-item>
			<u-form-item class="u-p-l-40" label-width="140" label-position="left" label="民族" prop="stuMZ">
				<u-input :border="border" placeholder="请输入民族" v-model="user.stuMz" type="text"></u-input>
			</u-form-item>
			<u-form-item class="u-p-l-40" label-width="140" label-position="left" label="政治面貌" prop="stuZZMM">
				<u-input :border="border" placeholder="请输入政治面貌" v-model="user.stuZzmm" type="text"></u-input>
			</u-form-item>
			<u-form-item class="u-p-l-40" label-width="140" label-position="left" label="详细地址" prop="stuDiZhi">
				<u-input :border="border" placeholder="请输入详细地址" v-model="user.stuDizhi" type="text"></u-input>
			</u-form-item>
		<!-- 	<u-form-item class="u-p-l-40" label-width="140" label-position="left" label="报道日期" prop="baoDaoDate">
				<u-input :border="border" placeholder="请输入报道日期"  v-model="user.baodaoDate" type="text"></u-input><!-- 注意调用修改 -->
			<!-- </u-form-item> -->
			<u-form-item class="u-p-l-40" label-width="140" label-position="left" label="手机号码" prop="stuNum">
				<u-input :border="border" placeholder="请输入手机号码"  v-model="user.stuNum" type="text"></u-input><!-- 注意调用修改 -->
			</u-form-item>
			<u-form-item class="u-p-l-40" label-width="140" label-position="left" label="邮箱" prop="stuSHZ">
				<u-input :border="border" placeholder="请输入邮箱"  v-model="user.stuShz" type="text"></u-input><!-- 注意调用修改 -->
			</u-form-item>
			<u-form-item class="u-p-l-40" label-width="140" label-position="left" label="兴趣爱好" prop="aihao">
				<u-input :border="border" placeholder="请输入兴趣爱好" v-model="user.aiHao" type="text"></u-input>
			</u-form-item>
			<u-form-item class="u-p-l-40" label-width="140" label-position="left" label="特长" prop="techang">
				<u-input :border="border" placeholder="请输入特长" v-model="user.teChang" type="text"></u-input>
			</u-form-item>
		</u-form>
		<u-button @click="submit">提交</u-button>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				user:{},
				border:true,
			}
		},
		methods: {
			submit() {
				
				uni.request({
					url: 'http://localhost:8088/caiji',
					data: this.user,
					method: "POST",
					
					success: (res) => {
						if (res.data.code * 1 == 200) {
							uni.navigateBack()
						} else {
							this.$u.toast('更新失败')
						}
					}
				})
			},
		}
	}
</script>

<style>

</style>
