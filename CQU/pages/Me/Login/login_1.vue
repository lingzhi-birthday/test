<!-- <template>
	<view class="wrap">
		<u-form :model="user" ref="uForm">
			<u-form-item left-icon="account" label-width="120" label="学号" prop="stuId">
				<u-input placeholder="请输入学号" v-model="user.stuId" type="text"></u-input>
			</u-form-item>
			<u-form-item left-icon="lock" label-width="120" label="密码" prop="stuCode">
				<u-input :password-icon="true" type="password" v-model="user.stuCode" placeholder="请输入密码"></u-input>
			</u-form-item>

		</u-form>
		<view> <u-button @click="submit">登录</u-button></view>
		<view class="u-flex u-row-right u-p-t-40">
			<view @click="goToForget">忘记密码？</view>
		</view>
	</view>
</template> -->
<template>
  <view class="content" >
    <view class="header">
      <image src="/static/CQU.jpeg"></image>
    </view>

    <view class="list" ref="uForm" :model="user">
      <view class="list-call" prop="zhanghao">
        <image class="img" src="/static/icon/login/account.png"></image>
        <input class="sl-input" v-model="user.stuId" type="text" maxlength="11" placeholder="请输入学号" />
      </view>
      <view class="list-call" prop='mima'>
        <image class="img" src="/static/icon/login/password.png"></image>
        <input class="sl-input" v-model="user.stuCode" type="text" maxlength="32" placeholder="请输入密码" password="true" />
      </view>

    </view>

    <view class="button-login" hover-class="button-hover" @tap="submit">
      <text>登录</text>
    </view>

    <view class="agreenment">
	  <view class="u-flex u-row-right u-p-t-40">
	  	<view @click="goToForget">忘记密码？</view>
	  </view>
    </view>
  </view>
</template>

<script>
import loginVue from './login.vue';
	export default {
		data() {
			return {
				user: {
					stuId: '',
					stuCode: ''
				}
			}
		},
		methods: {
			goToForget() {
				uni.navigateTo({
					url: "/pages/Me/Login/forget"
				})
			},
			submit() {
				console.log(this.user,"****")
				uni.request({
					url: 'http://localhost:8088/studenglu',
					data: this.user,
					method: "POST",
					success: (res) => {
						if (res.data.code * 1 == 200) {
							try {
								uni.setStorageSync('user', res.data.result);
								uni.navigateBack()
							} catch (e) {
								this.$u.toast('身份信息格式异常')
							}
						} else {
							
							this.$u.toast('登陆失败，用户名密码错误')
						}
					}
				})
			}
		}
	}
</script>

<style>
  .content {
    display: flex;
    flex-direction: column;
    justify-content: center;
  }

  .header {
    width: 161rpx;
    height: 161rpx;
    background: rgba(63, 205, 235, 1);
    box-shadow: 0rpx 12rpx 13rpx 0rpx rgba(63, 205, 235, 0.47);
    border-radius: 50%;
    margin-top: 30rpx;
    margin-left: auto;
    margin-right: auto;
  }

  .header image {
    width: 161rpx;
    height: 161rpx;
    border-radius: 50%;
  }

  .list {
    display: flex;
    flex-direction: column;
    padding-top: 50rpx;
    padding-left: 70rpx;
    padding-right: 70rpx;
  }

  .list-call {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    height: 100rpx;
    color: #333333;
    border-bottom: 0.5px solid #e2e2e2;
  }

  .list-call .img {
    width: 40rpx;
    height: 40rpx;
  }

  .list-call .sl-input {
    flex: 1;
    text-align: left;
    font-size: 32rpx;
    margin-left: 16rpx;
  }

  .button-login {
    color: #FFFFFF;
    font-size: 34rpx;
    width: 470rpx;
    height: 100rpx;
    background: linear-gradient(-90deg, rgba(63, 205, 235, 1), rgba(188, 226, 158, 1));
    box-shadow: 0rpx 0rpx 13rpx 0rpx rgba(164, 217, 228, 0.2);
    border-radius: 50rpx;
    line-height: 100rpx;
    text-align: center;
    margin-left: auto;
    margin-right: auto;
    margin-top: 100rpx;
  }

  .button-hover {
    background: linear-gradient(-90deg, rgba(63, 205, 235, 0.8), rgba(188, 226, 158, 0.8));
  }

  .agreenment {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    font-size: 30rpx;
    margin-top: 80rpx;
    color: #FFA800;
    text-align: center;
    height: 40rpx;
    line-height: 40rpx;
  }

  .agreenment text {
    font-size: 24rpx;
    margin-left: 15rpx;
    margin-right: 15rpx;
  }
</style>