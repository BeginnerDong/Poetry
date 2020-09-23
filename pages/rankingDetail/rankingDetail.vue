<template>
	<view>
		
		<image src="../../static/images/img1.png" mode="widthFix" class="bgImg"></image>
		
		<view class="p-r line-h">
			
			<view class="p-3">
				<view class="font-40 font-w">鹅鹅鹅</view>
				<view class="font-24 pt-2 color9">背诵主题</view>
				
				<button class="Mgb colorf font-26 flex0 p-a share" open-type="share">
					<image src="../../static/images/list-icon2.png" class="wh30 mr-1"></image>
					<view>分享</view>
				</button>
			</view>
			
			
			<view class="flex p-3 font-24" v-for="(item,index) in 5" :key="index">
				<image src="../../static/images/list-icon3.png" class="icon mr-4" v-show="index==0"></image>
				<image src="../../static/images/list-icon4.png" class="icon mr-4" v-show="index==1"></image>
				<image src="../../static/images/list-icon5.png" class="icon mr-4" v-show="index==2"></image>
				<view class="icon font-40 mr-4 font-w" v-show="index>2">{{index+1}}</view>
				<image src="../../static/images/my-img.png" class="wh80 radius-5"></image>
				<view class="flex-1 pl-2">
					<view class="font-26 color6 pb-2">赵同学</view>
					<view>背诵时长03:15</view>
				</view>
				<view class="colorM font-30">我</view>
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
.icon{width: 30rpx;height: 40rpx;}
</style>
