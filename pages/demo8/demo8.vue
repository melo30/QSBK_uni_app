<template>
	<view>
		<view class="font">
			{{ZHWeight}}
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				// 体重
				weight:1200
			}
		},
		// 计算属性
		computed: {
			ZHWeight () {
				return (this.weight>1000)?(this.weight/1000) + 'kg': this.weight + 'g';
			}
		},
		methods: {
			
		}
	}
</script>

<style>
	.font {
		font-size: 50upx;
	}
</style>
