<template>
	<view>
		
		<image src="../../static/images/img1.png" mode="widthFix" class="bgImg"></image>
		
		<view class="p-r text-c">
			
			<view class="font-24 flex4 p-a color9 px-3 pt-5">
				<image src="../../static/images/details-icon5.png" class="wh34"></image>
				<!-- <image src="../../static/images/details-icon7.png" class="wh34"></image> -->
				<view>收藏</view>
			</view>
			
			<view class="pt-5 font-40 line-h">今离别（其一）</view>
			<view class="pt-2 pb-4">清代·黄遵宪</view>
			
			<view class="px-3 line-h-lg font-34">
				别肠转如轮，一刻既万周。<br />
				眼见双轮驰，益增中心优。
			</view>
			
			<!-- 详情  开始背诵按钮-->
			<view v-show="type==0">
				<view style="height: 220rpx;"></view>
				<view class="py-2 bT-e1 flex0 p-fX bottom-0"
				@click="Router.navigateTo({route:{path:'/pages/info/info'}})">
					<image src="../../static/images/details-icon.png" class="wh160"></image>
					<view class="font-32 colorf p-r p-aX">背诵</view>
				</view>
			</view>
			
			<!-- 背诵过程按钮 -->
			<view v-show="type==1">
				<view style="height: 220rpx;"></view>
				<view class="py-2 bT-e1 flex2 p-fX bottom-0">
					<view class="flex4">
						<image src="../../static/images/details-icon2.png" class="wh56 mb-1"></image>
						<view class="font-32">回放</view>
					</view>
					<view @click="changeType(2)">
						<image src="../../static/images/details-icon1.png" class="icon"></image>
					</view>
					<view class="flex4">
						<image src="../../static/images/details-icon3.png" class="wh56 mb-1"></image>
						<view class="font-32">重录</view>
					</view>
				</view>
			</view>
			
			<!-- 回放展示 -->
			<!-- <view>
				<view style="height: 120rpx;"></view>
				<view class=" p-fX bottom-0 px-3 bT-e1">
					<view class="py-2 flex1">
						<image src="../../static/images/details-icon6.png" class="play-icon"></image>
						<view>
							<view class="p-r">
								<view class="line"></view>
								<view class="lineOn"></view>
							</view>
							<view class="line-h flex1 font-22 pt-2">
								<view>00:00/02:29</view>
								<view>错误率：<text class="colorM">8%</text></view>
							</view>
						</view>
						<view class="flex4" @click="changeType(1)">
							<image src="../../static/images/my-icon5.png" class="wh40 mb-1"></image>
							<view class="font-24 color6">报告</view>
						</view>
					</view>
				</view>
			</view> -->
			
			
			<!-- 背诵完成按钮 -->
			<view v-show="type==2">
				<view style="height: 220rpx;"></view>
				<view class=" p-fX bottom-0 px-3 bT-e1">
					<view class="py-2 flex1">
						<image src="../../static/images/details-icon6.png" class="play-icon"></image>
						<view>
							<view class="p-r">
								<view class="line"></view>
								<view class="lineOn"></view>
							</view>
							<view class="line-h flex1 font-22 pt-2">
								<view>00:00/02:29</view>
								<view>错误率：<text class="colorM">8%</text></view>
							</view>
						</view>
						<view class="flex4" @click="changeType(1)">
							<image src="../../static/images/details-icon3.png" class="wh56 mb-1"></image>
							<view class="font-32">重录</view>
						</view>
					</view>
					<view class="font-32 p-r pb-4 btn" @click="isShow">
						<image src="../../static/images/details-icon4.png" mode="widthFix"></image>
						<view class="p-aXY colorf flex0 pb-4">提交</view>
					</view>
				</view>
			</view>
			
			<!-- 背诵完成弹框 -->
			<view class="bg-mask flex0" v-show="is_show">
				<view class="mask p-r">
					<image src="../../static/images/complete-img1.png" class="wh250 mx-a nl"></image>
					<view class="font-30 pt-3 pb-5 mb-5">继续努力~</view>
					<view class="font-32 p-r pb-4 btn"
					@click="Router.navigateTo({route:{path:'/pages/report/report'}})">
						<image src="../../static/images/details-icon4.png" mode="widthFix"></image>
						<view class="p-aXY colorf flex0 pb-4">查看学习报告</view>
					</view>
					<view class="p-2 p-a top-0 right-0" @click="isShow">
						<image src="../../static/images/complete-icon.png" class="wh24"></image>
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
				Router:this.$Router,
				type:0,
				is_show:false
			}
		},
		onLoad(options) {
			const self = this;
			if(options.type){
				self.type = options.type;
			}
		},
		methods: {
			
			changeType(type){
				const self = this;
				self.type = type;
			},
			
			isShow(){
				const self = this;
				self.is_show = !self.is_show;
			}
			
		}
	}
</script>

<style scoped>
.wh56{width: 56rpx;height: 56rpx;}
.icon{width: 280rpx;height: 160rpx;}
.line{width: 510rpx;height: 8rpx;border-radius: 4rpx;background-color: #D2D2D2;}
.lineOn{height: 8rpx;border-radius: 4rpx;background-color: #BF2638;width: 20%;position: absolute;left: 0;top: 0;}
.lineOn::before{content: '';background-color: #BF2638;border-radius: 50%;width: 14rpx;height: 14rpx;border: 11rpx solid #F5A2AC;position: absolute;right: -18rpx;top: -10rpx;}

.mask{width: 600rpx;height: 700rpx;padding: 0 77rpx;}
.nl{margin-top: 120rpx;}
</style>
