<template>
	<view>
		
		<image src="../../static/images/img1.png" mode="widthFix" class="bgImg"></image>
		
		<view class="p-r px-3">
			
			<view class="flex py-4">
				<image src="../../static/images/my-img.png" class="wh120 radius-5"></image>
				<view class="pl-2">
					<view class="font-32 font-w mb-2">竹蜻蜓</view>
					<view class="sign"
					@click="Router.navigateTo({route:{path:'/pages/info/info'}})"></view>
					<!-- <view class="sign">诗词达人</view> -->
				</view>
			</view>
			
			<view class="flex p-r"
			@click="Router.navigateTo({route:{path:'/pages/info/info'}})">
				<image src="../../static/images/my-icon.png" class="wh54"></image>
				<view class="flex-1 flex bB-e1 py-4">
					<view class="flex-1 px-2">个人信息</view>
					<image src="../../static/images/my-icon7.png" class="R-icon"></image>
				</view>
			</view>
			<!-- 班主任 -->
			<view class="flex p-r"
			@click="Router.navigateTo({route:{path:'/pages/creatClass/creatClass'}})">
				<image src="../../static/images/my-icon1.png" class="wh54"></image>
				<view class="flex-1 flex bB-e1 py-4">
					<view class="flex-1 px-2">创建班级</view>
					<image src="../../static/images/my-icon7.png" class="R-icon"></image>
				</view>
			</view>
			<!-- 老师 ，班主任 -->
			<view class="flex p-r"
			@click="Router.navigateTo({route:{path:'/pages/public/public'}})">
				<image src="../../static/images/my-icon2.png" class="wh54"></image>
				<view class="flex-1 flex bB-e1 py-4">
					<view class="flex-1 px-2">布置作业</view>
					<image src="../../static/images/my-icon7.png" class="R-icon"></image>
				</view>
			</view>
			<!-- 老师 ，班主任-->
			<view class="flex p-r"
			@click="Router.navigateTo({route:{path:'/pages/collection/collection?type=3'}})">
				<image src="../../static/images/my-icon3.png" class="wh54"></image>
				<view class="flex-1 flex bB-e1 py-4">
					<view class="flex-1 px-2">学生作业</view>
					<image src="../../static/images/my-icon7.png" class="R-icon"></image>
				</view>
			</view>
			<!-- 学生 -->
			<view class="flex p-r"
			@click="Router.navigateTo({route:{path:'/pages/task/task'}})">
				<image src="../../static/images/my-icon3.png" class="wh54"></image>
				<view class="flex-1 flex bB-e1 py-4">
					<view class="flex-1 px-2">我的作业</view>
					<image src="../../static/images/my-icon7.png" class="R-icon"></image>
				</view>
				<view class="tag">1</view>
			</view>
			<!-- 家长 -->
			<view class="flex p-r"
			@click="Router.navigateTo({route:{path:'/pages/collection/collection?type=2'}})">
				<image src="../../static/images/my-icon3.png" class="wh54"></image>
				<view class="flex-1 flex bB-e1 py-4">
					<view class="flex-1 px-2">孩子学习报告</view>
					<image src="../../static/images/my-icon7.png" class="R-icon"></image>
				</view>
			</view>
			<view class="flex p-r"
			@click="Router.navigateTo({route:{path:'/pages/collection/collection?type=0'}})">
				<image src="../../static/images/my-icon4.png" class="wh54"></image>
				<view class="flex-1 flex bB-e1 py-4">
					<view class="flex-1 px-2">我的收藏</view>
					<image src="../../static/images/my-icon7.png" class="R-icon"></image>
				</view>
			</view>
			<view class="flex p-r"
			@click="Router.navigateTo({route:{path:'/pages/collection/collection?type=1'}})">
				<image src="../../static/images/my-icon5.png" class="wh54"></image>
				<view class="flex-1 flex bB-e1 py-4">
					<view class="flex-1 px-2">学习报告</view>
					<image src="../../static/images/my-icon7.png" class="R-icon"></image>
				</view>
			</view>
			<view class="flex p-r"
			@click="Router.navigateTo({route:{path:'/pages/message/message'}})">
				<image src="../../static/images/my-icon6.png" class="wh54"></image>
				<view class="flex-1 flex bB-e1 py-4">
					<view class="flex-1 px-2">留言反馈</view>
					<image src="../../static/images/my-icon7.png" class="R-icon"></image>
				</view>
			</view>
			
		</view>
		
		
		<view style="height: 130rpx;"></view>
		<!-- footer -->
		<view class="footer">
			<view class="item" @click="Router.redirectTo({route:{path:'/pages/index/index'}})">
				<image src="../../static/images/nabar1.png" mode=""></image>
				<view>首页</view>
			</view>
			<view class="item" @click="Router.redirectTo({route:{path:'/pages/ranking/ranking'}})">
				<image src="../../static/images/nabar2.png" mode=""></image>
				<view>排行榜</view>
			</view>
			<view class="item on">
				<image src="../../static/images/nabar3-a.png" mode=""></image>
				<view>我的</view>
			</view>
		</view>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				Router:this.$Router
			}
		},
		methods: {
			
		}
	}
</script>

<style>

</style>
