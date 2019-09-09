<template>
	<view>
		<!-- 这里  :class 的写法 可以在data里面实时的监听到class的变化 -->
		<view :class="classname">
			<view>{{username}}</view>
			<view>{{userinfo.username}}</view>
			<!-- <view>{{itemdata}}</view> -->
			
			<button type="primary" @tap="changeUserName('呵呵呵')">修改名字</button>
			<button type="primary" @tap="changeClass()">修改样式</button>
			
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				classname:"box2",
				username:"哈哈哈",
				userinfo:{
					username:"你是谁",
				}
			}
		},
		methods: {
			changeUserName:function (name) {
				this.username = name;
				this.userinfo.username = name + '傻逼';
			},
			changeClass:function () {
				this.classname = "box2";
			}
		}
	}
</script>

<style>
.box {
	border: 1upx solid #333333;
	height: 500upx;
	width: 100%;
	display: flex;
}

.box2 {
	border: 1upx solid #333333;
	height: 800upx;
	width: 100%;
	display: flex;
}

 /* 加个箭头代表 直选中box的下一级view，下下级是不会选中的！  而 .box view 中间没有箭头这样写代表选中box下面的所有东东 */
.box>view {
	background: #007AFF;
	color: #FFFFFF;
	font-weight: bold;
	font-size: 40upx;
	/* 每个元素占一份 */
	flex: 1;
	height: 500upx;
	
	display: flex;
	justify-content: center;
	align-items: center;
	border: 1upx solid #FFFFFF;
}
</style>
