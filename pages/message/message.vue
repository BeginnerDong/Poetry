<template>
	<view>
		
		<image src="../../static/images/img1.png" mode="widthFix" class="bgImg"></image>
		
		<view class="px-3 p-r">
			
			<view class="bg-white bB-e1 radius10 py-4">
				<view class="d-flex a-start">
					<image src="../../static/images/icon6.png" class="wh30 mt-1 mr-2"></image>
					<view class="avoidOverflow2 font-30 flex-1">position的值， relative和absolute分别是相对于谁进行定位的？</view>
				</view>
				<view class="d-flex a-start pt-1">
					<image src="../../static/images/icon7.png" class="wh28 mt-1 mr-2"></image>
					<view class="color6 flex-1">
						问题描述描述:position的值， relative和absolute分别是相对于谁进行定位的？position的值， relative和absolute分别是相对于谁进行定位的？position的值， relative和absolute分别是相对于谁进行定位的？
					</view>
				</view>
			</view>
			
			
			<view class="font-32 p-fX bottom-0 py-4 px-3"
			@click="Router.navigateTo({route:{path:'/pages/feedback/feedback'}})">
				<image src="../../static/images/details-icon4.png" mode="widthFix"></image>
				<view class="p-aXY colorf flex0">添加留言反馈</view>
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
.conImg{width: 610rpx;height: 280rpx;margin-top: 20rpx;}
.icon2{width: 30rpx;height: 30rpx;margin-right: 10rpx;margin-top: 10rpx;}
.icon3{width: 28rpx;height: 28rpx;position: absolute;left: 50rpx;}
</style>
