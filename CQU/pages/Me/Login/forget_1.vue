<template>
	<view class="wrap">
		<u-form :model="user" ref="uForm">
			<u-form-item label-width="140" label-position="left" label="学号" prop="stuId">
				<u-input :border="border" placeholder="请输入学号" v-model="user.stuId" type="text"></u-input>
			</u-form-item>
<!-- 			<u-form-item label-width="140" label-position="left" label="姓名" prop="stuName">
				<u-input :border="border" placeholder="请输入姓名" v-model="user.stuName" type="text"></u-input>
			</u-form-item> -->
			<u-form-item label-width="140" label-position="left" label="问题1" prop="stuDizhi">
				<u-input :border="border" placeholder="请问你的家在哪里？" v-model="user.stuDizhi" type="text"></u-input>
			</u-form-item>
			<u-form-item label-width="140" label-position="left" label="问题2" prop="stuDizhi">
				<u-input :border="border" placeholder="请问你的爱好是什么？" v-model="user.aiHao" type="text"></u-input>
			</u-form-item>
		</u-form>
		<view>
			<u-modal v-model="show" :content="content"></u-modal>
			<u-button @click="open">
				查询
			</u-button>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				border: true,
				user: {},
				mishi: "",
				show: false,
				content: 'sad'
			}
		},
		methods: {
			open() {
					// this.show = true;
					if(this.user.stuDizhi==null || this.user.aiHao==null){
						this.$u.toast("请回答问题")
						return
					}
					else{
						uni.request({
							url:'http://localhost:8088/chacode',
							data:this.user,
							method:"POST",
							success:(res)=>{
								if(res.data.code*1==200){
									try{
										this.content=res.data.result.stuCode;
										console.log(this.content);
										this.show=true;
									}catch(e){
										this.$u.toast('发生异常')
									}
									}else {
								this.$u.toast('查询错误')
							        }							
							}
						})
					}
		}
	}
	}
</script>

<style>
.wrap {
  padding: 20px;
}

.u-input {
  width: 100px;
}

.query-btn {
  margin-top: 20px;
}
</style>