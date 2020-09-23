<template>
	<view>
		
		<image src="../../static/images/img1.png" mode="widthFix" class="bgImg"></image>
		
		<view class="p-r px-3">
			
			<view class="bB-e1">
				<view class="font-34 line-h pt-4">背诵主题</view>
				<input type="text" value="" placeholder="请输入" />
			</view>
			<picker mode="selector">
				<view class="bB-e1">
					<view class="font-34 line-h pt-4">完成时间</view>
					<view class="flex1">
						<view class="txt">请选择</view>
						<image src="../../static/images/my-icon7.png" class="R-icon"></image>
					</view>
				</view>
			</picker>
			<picker mode="selector">
				<view class="bB-e1">
					<view class="font-34 line-h pt-4">选择班级</view>
					<view class="flex1">
						<view class="txt">请选择</view>
						<image src="../../static/images/my-icon7.png" class="R-icon"></image>
					</view>
				</view>
			</picker>
			
			
			<view class="font-32 p-fX bottom-0 btn">
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
input,.txt{font-size: 30rpx;height: 88rpx;line-height: 88rpx;}
.tt{width: 180rpx;height: 220rpx;margin-right: 20rpx;color: #888;}
</style>
