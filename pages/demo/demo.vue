<template>
	<view>
		<view class="view-box animated" hover-class="view-box-hover bounceIn">第一个view
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		}
	}
</script>

<style>
	.view-box {
		width: 200upx;
		height: 200upx;
		background: #007AFF;
		color: #FFFFFF;
		margin: 100upx;
	}
	.view-box-hover {
		background: red;
	}
</style>
