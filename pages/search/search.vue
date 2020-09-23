<template>
	<view>
		
		<image src="../../static/images/img1.png" mode="widthFix" class="bgImg"></image>
		
		<view class="py-2">
			<view class="flex font-24 color8 px-3 mx-3 p-r ss">
				<image src="../../static/images/home-icon.png" class="wh36 mr-3"></image>
				<input type="text" value="" placeholder="搜索想要找的商品" />
			</view>
		</view>
		
		<view class="line-h bB-e1 mx-3 pb-4 pt-7 p-r" v-for="(item,index) in 3" :key="index">
			<view class="flex1 pb-3">
				<view class="font-36">尽离别·其一</view>
				<view class="font-26">清代·黄遵宪</view>
			</view>
			<view class="font-30 avoidOverflow">别肠转如轮，一刻既万周。眼见双轮驰，益增中心忧。古亦有山川，古亦有车舟。</view>
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
.pt-7{padding-top: 70rpx;}
input{padding: 0;flex: 1;}
</style>
