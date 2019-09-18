<template>
	<view>
		<view class="index-list">
			<view class="index-list1 u-f-ac">
				<view class="u-f-ac">
						<image src="../../static/头像.png" mode="aspectFill" lazy-load></image>
						昵称
				</view>
				<view class="u-f-ac">
					<view></view>+ 关注
				</view>
			</view>
			<view class="index-list2">我是标题</view>
			<view class="index-list3">
				<image src="../../static/风景.png" mode="widthFix" lazy-load=""></image>
			</view>
			<view class="index-list4 u-f-ac">
				<view class="u-f-ac">
					<view class="u-f-ac"><image src="../../static/笑脸.png" mode="widthFix"></image>10</view>
					<view class="u-f-ac"><image src="../../static/哭脸.png" mode="widthFix"></image>10</view>
				</view>
				
				<view class="u-f-ac">
					<view class="u-f-ac"><image src="../../static/评论.png" mode="widthFix"></image>10</view>
					<view class="u-f-ac"><image src="../../static/点赞.png" mode="widthFix"></image>10</view>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang="scss">
	.u-f, .u-f-ac,.u-f-ajc{
		display: flex;
	}
	.u-f-ac , .u-f-ajc{
		align-items: center;
	}
	.u-f-ajc {
		justify-content: center;
	}
	.index-list {
		padding: 10upx;
		border-bottom: 1upx solid #999999;
	}
	.index-list1 {
		justify-content: space-between;
	}
	.index-list1>view:first-child {
		color: #999999;
		font-size: 10upx;
	}
	.index-list1>view:first-child image{
		width: 40upx;
		height: 40upx;
		border-radius: 100%;
		margin-right: 10upx;
	}
	.index-list1>view:last-child {
		background: #F5f5f5;
		border-radius: 5upx;
		font-size: 10upx;
		padding: 0 5upx;
	}
	.index-list1>view:last-child>view {
		
	}
	.index-list2 {
		padding-top: 5upx;
		font-size: 12upx;
		color: #333333;
	}
	.index-list3 {
		padding-top: 0upx;
	}
	.index-list3>image {
		width: 100%;
		border-radius: 5upx;
	}
	.index-list4 {
		padding: 0upx 0;
		justify-content: space-between;
	}
	.index-list4>view {
		color: #999999;
	}
	.index-list4>view>view {
		font-size: 10upx;
	}
	.index-list4 image {
		width: 10upx;
		height: 10upx;
	}
</style>
