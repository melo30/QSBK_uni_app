<template>
	<view>
		<!-- <view class="view-box animated" hover-class="view-box-hover bounceIn">第一个view
		</view> -->
		
		
		<!-- <view class="box">
			<text>text组件</text>
			<view>1</view>
			<view>2</view>
			<view>3</view>
			<view>4</view>
			<view>5</view>
			<view>6</view>
			<view>7</view>
		</view> -->
		
		<view class="box">
			<view class="box-item">1</view>
			<view class="box-item">2</view>
			<view class="box-item">3</view>
			<!-- <view class="box-item">4</view>
			<view class="box-item">5</view>
			<view class="box-item">6</view> -->
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
	.box {
		height: 500upx;
		width: 100%;
		border: 1upx solid #333333;
		
		/* flex布局,不会自动去换行,无论多少会挤到同一行*/
		display: flex;
		/* flex-direction: column; */
		/* justify-content: center; */
		/* align-items: center; */
		
	}
	.box-item {
		background: #007AFF;
		color: #FFFFFF;
		height: 200upx;
		flex: 1;
		/* width: 50%; */
		/* width: 200upx; */
		font-size: 30upx;
		font-weight: bold;
		text-align: center;
	}
	
	/* 偶数选择器 */
	.box-item:nth-of-type(even) {
		background: #007AFF;
	}
	/* 奇数选择器 */
	.box-item:nth-of-type(odd) {
		background: #09BB07;
	}
	.box-item:nth-of-type(1) {
		flex: 1;
	}
	.box-item:nth-of-type(2) {
		flex: 2;
		align-self: flex-end;
	}
	.box-item:nth-of-type(3) {
		flex: 1;
	}
/* 	设置第一项不会被压缩
	.box-item:first-of-type {
		flex-shrink: 0;
	} */
</style>
