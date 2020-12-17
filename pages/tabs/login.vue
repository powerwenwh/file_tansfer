<template>
	<view>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				userphone: '',
				userpw: ''
			}
		},
		methods: {
			login: async function() {
				if (!this.userphone || !this.userpw) {
					uni.showToast({
						title: "账号或者密码不能为空",
						icon: 'none',
						duration: 2000,
					});
				} else {
					var [error, res] = await uni.request({
						url: 'https://httpbin.org/anything', 
						data: {
							phone: this.userphone,
							password: this.userpw
						}
					});
					console.log(res);
				}
			
			}
			
		}
	}
</script>

<style>

</style>
