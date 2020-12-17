<template>
	<view class="center">
		<view class="logo">
			<image class="logo-img" :src="avatarUrl"></image>
			<text class="uer-name">Hi，您未登录</text>
		</view>
		<view class="btn-row">
			<button  class="primary" >退出登录</button>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				avatarUrl: "../../static/img/logo.png",
			}
		},
		methods: {
			
		}
	}
</script>

<style>
	.logo {
		width: 750rpx;
		height: 240rpx;
		padding: 20rpx;
		box-sizing: border-box;
		background-color: #0faeff;
		flex-direction: row;
		align-items: center;
	}
	
	.logo-img {
		width: 120rpx;
		height: 120rpx;
		border-radius: 150rpx;
	}
	
	.logo-title {
		height: 150rpx;
		flex: 1;
		align-items: center;
		justify-content: space-between;
		flex-direction: row;
		margin-left: 20rpx;
	}
	
	.uer-name {
		height: 60rpx;
		line-height: 60rpx;
		color: #FFFFFF;
	}
</style>
