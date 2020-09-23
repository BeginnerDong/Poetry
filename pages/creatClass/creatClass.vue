<template>
	<view>
		
		<image src="../../static/images/img1.png" mode="widthFix" class="bgImg"></image>
		
		<view class="p-r px-3">
			
			<view class="bB-e1">
				<view class="font-34 line-h pt-4">年级班级</view>
				<input type="text" value="" placeholder="请输入" />
			</view>
			<view class="bB-e1">
				<view class="font-34 line-h pt-4">人数</view>
				<input type="text" value="" placeholder="请输入" />
			</view>
			<view class="bB-e41 pb">
				<view class="font-34 line-h pt-4">信息导入</view>
				<view class="flex flex-wrap">
					<view class="flex0 bg-f5 radius10 mt-3 tt">
						<image src="../../static/images/create-icon.png" class="wh60"></image>
					</view>
				</view>
			</view>
			
			
			<view class="font-32 p-fX bottom-0 btn"
			@click="Router.navigateTo({route:{path:'/pages/user/user'}})">
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
.tt{width: 180rpx;height: 220rpx;margin-right: 20rpx;}

.btn{margin: 40rpx  0;}
</style>
