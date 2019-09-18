<template>
	<view>
		<view class="index-list">
			<view class="index-list1 u-f-ac u-f-jsb">
				<view class="u-f-ac">
						<image src="../../static/头像.png" mode="aspectFill" lazy-load></image>
						陈诚
				</view>
				<view class="u-f-ac">
					<view></view>+ 关注
				</view>
			</view>
			<view class="index-list2">这里是标题</view>
			<view class="index-list3">
				<image src="../../static/风景.png" mode="widthFix" lazy-load=""></image>
			</view>
			<view class="index-list4 u-f-ac u-f-jsb">
				<view class="u-f-ac">
					<view class="u-f-ac"><image src="../../static/笑脸.png" mode="aspectFit"></image>10</view>
					<view class="u-f-ac"><image src="../../static/哭脸.png" mode="aspectFit"></image>10</view>
				</view>
				
				<view class="u-f-ac">
					<view class="u-f-ac"><image src="../../static/评论.png" mode="aspectFit"></image>10</view>
					<view class="u-f-ac"><image src="../../static/点赞.png" mode="aspectFit"></image>10</view>
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
	.index-list {
		padding: 20upx;
		border-bottom: 1upx solid #E0E0E0;
	}
	.index-list1>view:first-child {
		color: #999999;
		font-size: 30upx;
	}
	.index-list1>view:first-child image{
		width: 90upx;
		height: 90upx;
		border-radius: 100%;
		margin-right: 20upx;
	}
	.index-list1>view:last-child {
		background: #F5f5f5;
		border-radius: 10upx;
		font-size: 30upx;
		padding: 0 20upx;
	}
	.index-list2 {
		padding-top: 10upx;
		font-size: 30upx;
		color: #333333;
	}
	.index-list3 {
		padding-top: 20upx;
	}
	.index-list3>image {
		width: 100%;
		border-radius: 10upx;
	}
	.index-list4 {
		padding: 10upx 0;
	}
	.index-list4>view {
		color: #999999;
	}
	.index-list4>view>view {
		font-size: 30upx;
	}
	.index-list4 image {
		width: 30upx;
		height: 30upx;
	}
</style>
