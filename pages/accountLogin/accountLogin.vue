<template>
	<view>
		<view class="logo"><image src="../../static/studyCatAccount.svg" mode="widthFix"></image></view>
		<view class="accountLogin-container">
			<input type="text" placeholder="账号" v-model="account" class="accountLogin-account" />
			<input type="password" placeholder="密码" v-model="password" class="accountLogin-password" />
			<button class="accountLogin-btn" @click="login()">登录</button>
		</view>
		<view class="another-login">
			<text class="anthor-login-text">其他登录方式</text>
			<image src="../../static/wechat.svg" class="login-logo" mode="widthFix" @click="wechatLogin()"></image>
		</view>
	</view>
</template>

<script>
export default {
	data() {
		return {
			account: '',
			password: ''
		};
	},
	methods: {
		login(){
			uni.redirectTo({
				
			})
		},
		wechatLogin(){
			console.log('ss')
			uni.redirectTo({
				url:'/pages/login/login'
			})
		}
	}
};
</script>

<style lang="less">
@import url('accountLogin.less');
</style>
