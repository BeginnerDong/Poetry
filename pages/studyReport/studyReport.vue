<template>
	<view>
		
		<image src="../../static/images/img1.png" mode="widthFix" class="bgImg"></image>
		
		<view class="p-r line-h">
			
			<view class="py-5 line-h text-c font-40 font-w">今别离·其一</view>
			
			
			<view class="flex p-3 font-24" v-for="(item,index) in 5" :key="index">
				<image src="../../static/images/ranking-icon.png" class="icon mr-4" v-show="index==0"></image>
				<image src="../../static/images/ranking-icon1.png" class="icon mr-4" v-show="index==1"></image>
				<image src="../../static/images/ranking-icon2.png" class="icon mr-4" v-show="index==2"></image>
				<view class="icon font-40 mr-4 font-w" v-show="index>2">{{index+1}}</view>
				<image src="../../static/images/my-img.png" class="wh80 radius-5"></image>
				<view class="flex-1 pl-2">
					<view class="font-26 pb-2">赵同学</view>
					<view class="flex1">
						<view>
							<view>完成时间:2020.08.23 12:00</view>
							<view class="flex pt-2">
								<view class="pr-3">班级排行: <text class="colorM">1</text></view>
								<view>年级排行: <text class="colorM">10</text></view>
							</view>
						</view>
						<view>
							<view>背诵时长:03:15</view>
							<view class="pt-2">错误率: <text class="colorM">0%</text></view>
						</view>
					</view>
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
.share{width: 140rpx;line-height: 50rpx;right: 0;top: 50rpx;border-radius: 25rpx 0 0 25rpx;}
.icon{width: 46rpx;height: 38rpx;}
</style>
