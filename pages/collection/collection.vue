<template>
	<view>
		
		<image src="../../static/images/img1.png" mode="widthFix" class="bgImg"></image>
		
		<view class="line-h bB-e1 mx-3 pb-4 pt-7 p-r" v-for="(item,index) in 3" :key="index"
		@click="goDetail">
			<view class="flex1 pb-3">
				<view class="font-36">尽离别·其一</view>
				<view class="font-26" v-show="type==0">清代·黄遵宪</view>
			</view>
			<view class="font-30 avoidOverflow" v-show="type==0">别肠转如轮，一刻既万周。眼见双轮驰，益增中心忧。古亦有山川，古亦有车舟。</view>
			<view class="font-26 color6 flex1" v-show="type!=0">
				<view>完成时间：2020.08.12 12:00</view>
				<view class="color9">背诵时长：12:00</view>
			</view>
		</view>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				Router:this.$Router,
				type:0
			}
		},
		onLoad(options) {
			const self = this;
			if(options.type){
				if(options.type==1){
					self.changeTit('学习报告')
				}
				if(options.type==2||options.type==3){
					self.changeTit('孩子学习报告')
				}
			}
			self.type = options.type;
		},
		methods: {
			
			changeTit(title){
				uni.setNavigationBarTitle({
				    title: title
				});
			},
			
			goDetail(){
				const self = this;
				if(self.type==3){
					self.Router.navigateTo({route:{path:'/pages/studyReport/studyReport'}})
				}else{
					self.Router.navigateTo({route:{path:'/pages/poemsDetail/poemsDetail'}})
				}
			}
			
		}
	}
</script>

<style>

</style>
