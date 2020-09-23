<template>
	<view>
		
		<image src="../../static/images/img1.png" mode="widthFix" class="bgImg"></image>
		
		<view class="p-r flex4">
			
			<image src="../../static/images/my-img.png" class="wh140 radius-5 tx"></image>
			<view class="py-3">商胜负</view>
			
			<view class="font-36 font-w pt-5">今别离（其一）</view>
			<view class="font-24 color9 pt-2">背诵主题</view>
			
			<view class="flex0">
				
				<view class="my-5 p-r colorf line-h">
					<image src="../../static/images/details-icon7.png" class="pm"></image>
					<view class="flex4 p-aXY">
						<view class="font-50 font-w">5</view>
						<view class="font-24 pt-1">排名</view>
					</view>
				</view>
				<!-- 学生展示两个 -->
				<!-- <view class="my-5 p-r colorf line-h ml-5">
					<image src="../../static/images/details-icon7.png" class="pm"></image>
					<view class="flex4 p-aXY">
						<view class="font-50 font-w">5</view>
						<view class="font-24 pt-1">排名</view>
					</view>
				</view> -->
				
			</view>
			
			<view class="flex1 line-h px-3 pt-5 w-100">
				<view class="flex4 w-33 rb">
					<view class="font-30 pb-2">2020.08.12</view>
					<view class="font-24 color6">背诵日期</view>
				</view>
				<view class="flex4 w-33 rb">
					<view class="font-30 pb-2">12:02:02</view>
					<view class="font-24 color6">开始时间</view>
				</view>
				<view class="flex4 w-33">
					<view class="font-30 pb-2">12:04:02</view>
					<view class="font-24 color6">结束时间</view>
				</view>
			</view>
			<view class="flex1 line-h px-3 pt-4 w-100">
				<view class="flex4 w-50 rb">
					<view class="font-30 pb-2">02:09</view>
					<view class="font-24 color6">完成时长</view>
				</view>
				<view class="flex4 w-50">
					<view class="font-30 pb-2">0%</view>
					<view class="font-24 color6">错误率</view>
				</view>
			</view>
			
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

<style scoped>
.tx{box-shadow: 0 4rpx 10rpx 0 rgba(0,0,0,0.2);margin-top: 100rpx;}
.pm{width: 310rpx;height: 295rpx;}
</style>
