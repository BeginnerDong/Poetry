<template>
	<view>
		
		<image src="../../static/images/img1.png" mode="widthFix" class="bgImg"></image>
		
		<view class="p-r pt-5">
			
			<view class="flex flex-wrap text-c bT-e1">
				<block v-for="(item,index) in 9" :key="index">
					<view class="w-33 px-5 font-26 flex0 bB-e1 bR-e1 txt"
					@click="Router.navigateTo({route:{path:'/pages/rankingDetail/rankingDetail'}})">小学生古诗词背诵</view>
				</block>
			</view>
			
			<view class="page">
				<image src="../../static/images/list-icon.png" class="pageL"></image>
				<view class="pageLi on">1</view>
				<view class="pageLi">2</view>
				<view class="pageLi">3</view>
				<image src="../../static/images/list-icon1.png" class="pageR"></image>
			</view>
			
		</view>
		
		
		
		<view style="height: 130rpx;"></view>
		<!-- footer -->
		<view class="footer">
			<view class="item" @click="Router.redirectTo({route:{path:'/pages/index/index'}})">
				<image src="../../static/images/nabar1.png" mode=""></image>
				<view>首页</view>
			</view>
			<view class="item on">
				<image src="../../static/images/nabar2-a.png" mode=""></image>
				<view>排行榜</view>
			</view>
			<view class="item" @click="Router.redirectTo({route:{path:'/pages/user/user'}})">
				<image src="../../static/images/nabar3.png" mode=""></image>
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

<style scoped>
.txt{height: 250rpx;}
.txt:nth-child(3n){border-right: none;}

.page{margin-top: 100rpx;}
</style>
