<template>
	<view class="imfo">
		<u-form :model="user" ref="uForm">
			<u-input v-show="false" v-model="user.stuId" type="text"></u-input>
			<uni-card title="姓名">
				<text><u-input v-model="user.stuName" type="text"></u-input></text>
			</uni-card>
			<uni-card title="学号">
				<text>{{user.stuId}}</text>
			</uni-card>
			<uni-card title="班级">
				<text>{{user.claId}}</text>
			</uni-card>
			<uni-card title="年级">
				<text>{{user.stuNj}}</text>
			</uni-card>
			<uni-card title="性别">
				<text>{{user.stuSex}}</text>
			</uni-card>
			<uni-card title="民族">
				<text>{{user.stuMz}}</text>
			</uni-card>
			<uni-card title="政治面貌">
				<text>{{user.stuZzmm}}</text>
			</uni-card>
			<uni-card title="详细地址">
				<text>{{user.stuDiZhi}}</text>
			</uni-card>
			<uni-card title="爱好">
				<text>{{user.aiHao}}</text>
			</uni-card>
			
			<uni-card title="特长">
				<text>{{user.teChang}}</text>
			</uni-card>
			<uni-card title="报道日期">
				<text>{{user.baodaoDate}}</text>
			</uni-card>
			<uni-card title="报道情况">
				<text>{{user.baodao}}</text>
			</uni-card>
			<uni-card title="联系电话">
				<text>{{user.stuNum}}</text>
			</uni-card>
<!-- 			<u-form-item class="u-p-l-40" label-width="140" label-position="left" label="学生姓名  :">{{user.Stu_Name}}</u-form-item>
			<u-form-item label-width="140" class="u-p-l-40" label-position="left" label="学号  :">{{user.Stu_id}}</u-form-item>
			<u-form-item class="u-p-l-40" label-width="140" label-position="left" label="班级  :">{{user.Cla_Id}}</u-form-item>
			<u-form-item class="u-p-l-40" label-width="140" label-position="left" label="年级  :">{{user.Stu_NJ}}</u-form-item>
			<u-form-item class="u-p-l-40" label-width="140" label-position="left" label="性别  :">{{user.Stu_Sex}}</u-form-item>
			<u-form-item class="u-p-l-40" label-width="140" label-position="left" label="民族  :">{{user.Stu_MZ}}</u-form-item>
			<u-form-item class="u-p-l-40" label-width="140" label-position="left" label="政治面貌  :">{{user.Stu_ZZMM}}</u-form-item>
			<u-form-item class="u-p-l-40" label-width="140" label-position="left" label="详细地址  :">{{user.Stu_DiZhi}}</u-form-item>
			<u-form-item class="u-p-l-40" label-width="140" label-position="left" label="兴趣爱好  :">{{user.AiHao}}</u-form-item>
			<u-form-item class="u-p-l-40" label-width="140" label-position="left" label="特长  :">{{user.TeChang}}</u-form-item>
			<! <u-form-item class="u-p-l-40" label-width="140" label-position="left" label="学生类别  :">{{user.Stu_Type}}
			<u-radio-group v-model="user.Stu_Type" @change="radioGroupChange">
				<u-radio @change="radioChange" v-for="(item, index) in list" :key="index" :name="item.name"
					:disabled="item.disabled">
					{{item.txt}}
				</u-radio>
			</u-radio-group>
			</u-form-item> -->
<!-- 			<u-form-item class="u-p-l-40" label-width="140" label-position="left" label="报道日期  :">{{user.BaoDao_Date}}</u-form-item>
			<u-form-item class="u-p-l-40" label-width="140" label-position="left" label="报道情况  :">{{user.BaoDao}}</u-form-item>
			<u-form-item class="u-p-l-40" label-width="140" label-position="left" label="联系电话  :">{{user.Stu_Num}}</u-form-item> --> 
			</u-form>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				border: true,
				user: {},
				list: [{
						name: '0',
						txt: "非特长生",
						disabled: true
					},
					{
						name: '1',
						txt: "艺术生",
						disabled: true
					},
					{
						name: '2',
						txt: "体育生",
						disabled: true
					}
				]
			}
		},
		onLoad(canshu) {
			console.log(canshu,"*xx***")
			uni.request({
				url: `http://localhost:8088/jibenInfo/${canshu.stuId}`,
				
				success: (res) => {
					if (res.data.code * 1 == 200) {
						console.log(res.data,"########")
						this.user = res.data.result
						
						console.log(user,"USER******")
					}
				}
			})
		},
		methods: {
			radioChange(e) { 
					console.log(e,"radio") 
			},
			radioGroupChange(e){
				console.log(e,"group")
			}
		}
	}
</script>

<style>
	.info{
		padding: 5px 30px;
	}
</style>