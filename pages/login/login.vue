<template>
	<view>
		<view class="logo"><image src="../../static/studyCat.svg" mode="widthFix"></image></view>
		<button class="login-btn" @click="login()">
			<image mode="widthFix" src="../../static/wx.svg"></image>
			微信登录
		</button>
		<view class="register"><text class="register-link" @click="accountLogin()">账号登录</text></view>
	</view>
</template>

<script>
export default {
	data() {
		return {};
	},
	methods: {
		accountLogin() {
			console.log("sss");
			uni.redirectTo({
				url:'/pages/accountLogin/accountLogin'
			})
		}
	}
};
</script>

<style lang="less">
@import url(login.less);
</style>
