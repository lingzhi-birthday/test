<template>
	<view>
		<view v-if="logined">
			<u-navbar :is-back="false" title=" " :border-bottom="false">
				<view class="u-flex u-row-right" style="width: 100%;">
					<view class="camera u-flex u-row-center">
						<u-icon name="camera-fill" color="#000000" size="48">
						</u-icon>
					</view>
				</view>
			</u-navbar>
			<view class="u-flex user-box u-p-l-40 u-p-r-10 u-p-b-10">
				<view class="u-m-r-30">
					<u-avatar src="../../static/images/personal.png" size="100"></u-avatar>
				</view>
				<view class="u-flex-1">
					<view class="u-font-40 u-p-b-0">姓名：{{user.stuName}}</view>
					<view class="u-font-10 u-tips-color">学号：{{user.stuId}}</view>
				</view>
				<view class="u-m-l-10 u-p-10">
					<u-icon name="scan" color="#969799" size="0"></u-icon>
				</view>
				<view class="u-m-l-10 u-p-10">
					<u-icon name="arrow-right" color="#969799" size="28"></u-icon>
				</view>
			</view>
			<view class="u-m-t-20 u-p-0">
				<u-cell-group>
					<u-cell-item icon="account" title="我的信息" @click="goTomyinfo"></u-cell-item>
					<u-cell-item icon="man-add" title="修改信息" @click="goTocollect"></u-cell-item>
					<!-- <u-cell-item icon="man-add-fill" title="修改信息" @click="goTochangeinfo"></u-cell-item> -->
					<u-cell-item icon="reload" title="修改密码" @click="goTochangepassword"></u-cell-item>
				</u-cell-group>
			</view>
			<view class="u-m-t-20">
				<u-cell-group>
					<u-cell-item icon="man-delete" title="退出登录" @click="quit"></u-cell-item>
				</u-cell-group>
			</view>
		</view>
		<view v-else>
			<u-navbar :is-back="false" title=" " :border-bottom="false">
				<view class="u-flex u-row-right" style="width: 100%;">
					<view class="camera u-flex u-row-center">
						<u-icon name="camera-fill" color="#000000" size="48">
						</u-icon>
					</view>
				</view>
			</u-navbar>
			<view class="u-flex user-box u-p-l-30 u-p-r-20 u-p-b-30">
				<view class="u-m-r-10">
					<u-avatar src="../../static/images/personal.png" size="140"></u-avatar>
				</view>
				<view class="u-flex-1">
					<view class="u-font-19 u-p-b-10">学生</view>
					<view class="u-font-13 u-tips-color">请登录</view>
				</view>
			</view>
			<view class="u-m-t-20" @click="goTologin()">
				<u-cell-group>
					<u-cell-item icon="man-add"  title="登录"></u-cell-item>
				</u-cell-group>
			</view>
		</view>
	</view>
</template>
<script>
	export default {
		data() {
			return {
				logined: false,
				user: {
					// stuName: "user.Stu_Name",
					// stuId:"user.Stu_Id",
				}
			}
		},
		onShow() {
			try {
				const value = uni.getStorageSync('user')
				console.log("onshow", value)
				if (value) {
					this.logined = true
					this.user = value
				} else {
					this.logined =false
				}
			} catch (e) {}
		}, 
		methods: {
			goTomyinfo() {
				uni.navigateTo({
					url: "/pages/Me/Info/myinfo?stuId="+this.user.stuId,
				})
			},
			// goTochangeinfo() {
			// 	uni.navigateTo({
			// 		url: "/pages/CQU/changeinfo"
			// 	})
			// },
			goTochangepassword() {
				uni.navigateTo({
					url: "/pages/Me/changepassword?stuId="+this.user.stuId,
				})
			},
			goTocollect() {
				uni.navigateTo({
					url: "/pages/Me/Info/xiugaiinfo?stuId="+this.user.stuId,
				})
			},
			goTologin() {
				uni.navigateTo({
					url: "/pages/Me/Login/login"
				})
			},
			quit() {
				uni.setStorageSync("user", "")
				this.logined = false
			}
		}
	}
</script>

<style>

</style>