<template>
	<view>
		
		<image src="../../static/images/img1.png" mode="widthFix" class="bgImg"></image>
		
		<view class="p-r">
			
			<textarea value="" placeholder="请描述你遇到的问题或者给我们建议..." />
			<view class="f5Bj-H20"></view>
			
			<view class="bB-e1 mx-3">
				<view class="font-34 line-h pt-4 color9">客服微信号</view>
				<view class="txt">shsci123456</view>
			</view>
			
			<view class="font-32 p-fX bottom-0 py-4 px-3"
			@click="Router.navigateTo({route:{path:'/pages/feedback/feedback'}})">
				<image src="../../static/images/details-icon4.png" mode="widthFix"></image>
				<view class="p-aXY colorf flex0">确定</view>
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
textarea{width: 100%;height: 480rpx;padding: 30rpx;font-size: 28rpx;}
.txt{font-size: 30rpx;height: 88rpx;line-height: 88rpx;}
</style>
