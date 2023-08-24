<template>
	<view class="wrap">
		<u-form :model="user" ref="uForm">
			<u-input v-show="false" v-model="user.stuId" type="text"></u-input>
			<u-form-item class="u-p-l-40" label-width="150" label-position="left" label="学号  :" prop="stuId">
				<u-input :border="border" placeholder="请输入学号" v-model="user.stuId"
					type="text"></u-input><!-- 注意调用修改 -->
			</u-form-item>
			 <u-form-item label-width="150" label-position="left" label="原密码" prop="stulCode1"style="margin-left: 20px;">
					<u-input :border="border" placeholder="请输入原密码" v-model="user.stulCode1"
						type="text"></u-input><!-- 注意调用修改 -->
				</u-form-item>
					
			</u-form-item> 
			<u-form-item class="u-p-l-40" label-width="150" label-position="left" label="新密码" prop="stuCode">
				<u-input :border="border" type="password" v-model="user.sturCode"
					placeholder="请输入密码"></u-input><!-- 注意调用修改 -->
			</u-form-item>
			<u-form-item class="u-p-l-40" label-width="150" label-position="left" label="确认新密码" prop="stu_r2Code">
				<u-input :border="border" type="password" v-model="user.stur2Code"
					placeholder="再输一次密码"></u-input><!-- 注意调用修改 -->
			</u-form-item>
		</u-form>
		<u-button @click="submit">提交</u-button>
	</view>
</template>


<script>
	export default {
		data() {
			return {
				user: {
					// Stu_id:"",
					// /* Stu_Code:"", */
					// Stu_r1Code:"",
					// Stu_r2Code:""
				},
				stulCode:{},
				border: true,
				
			}
		},
		onLoad(canshu) {
			uni.request({
				url: `http://localhost:8088/chamima/${canshu.stuId}`,
				
				success: (res) => {
					if (res.data.code * 1 == 200) {
						
						this.stulCode = res.data.result
						
					}
					console.log(this.stulCode,"***")
				}
			})
		},
		
		methods: {
			submit() {
				console.log(this.user.sturCode )
				if (this.user.stulCode1 != this.stulCode.stuCode) {
						this.$u.toast("原密码错误，请重新输入")
						return
						} 
				else if (this.user.sturCode != this.user.stur2Code) {
					this.$u.toast("两次输入密码不同")
					return
					}
					else {
						console.log(this.user,"***"),
						uni.request({
							url: 'http://localhost:8088/xiugaimima',
							data: {
								stuId:this.user.stuId,
								stuCode:this.user.sturCode
								
							},
							method: "POST",
							success: (res) => {
								if (res.data.code * 1 == 200) {
									try {
										// uni.setStorageSync('user', res.data.result);
										uni.navigateBack()
									} catch (e) {
										this.$u.toast('身份信息格式异常')
									}
								} else {
									this.$u.toast('更改错误')
								}
							}
						})
					}
				}
			},
		}
</script>

<style>

</style>