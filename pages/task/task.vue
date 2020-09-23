<template>
	<view>
		
		<image src="../../static/images/img1.png" mode="widthFix" class="bgImg"></image>
		
		<view class="p-r line-h">
			
			<view class="p-s top-0">
				<view class="list">
					<view class="li" :class="liCurr==0?'colorM':''" @click="changeLi(0)">待完成(2)</view>
					<view class="li" :class="liCurr==1?'colorM':''" @click="changeLi(1)">已完成(2)</view>
					<view class="li" :class="liCurr==2?'colorM':''" @click="changeLi(2)">已过期(0)</view>
				</view>
				<view class="f5Bj-H20"></view>
			</view>
			
			<view class="flex1 mx-3 py-4 bB-e1">
				<view class="flex-1">
					<view class="font-30 pb-3 flex1">
						<view>今别离·其一</view>
						<view class="font-26 color9" v-show="liCurr==2">已过期</view>
					</view>
					<view class="font-26 color6 flex1">
						<view>完成时间：2020.08.12 12:00</view>
						<view class="color9" v-show="liCurr==1">背诵时长：12:00</view>
					</view>
				</view>
				<view class="font-24 colorf p-r bb" v-show="liCurr==0">
					<image src="../../static/images/task.png" ></image>
					<view class="p-aXY flex0">去完成</view>
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
				liCurr:0
			}
		},
		methods: {
			
			changeLi(index){
				const self = this;
				self.liCurr = index;
			}
			
		}
	}
</script>

<style scoped>
.list{background-color: initial;}
.li{width: 33.33%;font-size: 30rpx;}

.bb{width: 144rpx;height: 84rpx;}
.colorM{color: #BF2638;}
</style>
