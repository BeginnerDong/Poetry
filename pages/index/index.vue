<template>
	<view>
		
		<image src="../../static/images/img1.png" mode="widthFix" class="bgImg"></image>
		
		<view class="py-2">
			<view class="flex font-24 color8 px-3 mx-3 p-r ss"
			@click="Router.navigateTo({route:{path:'/pages/search/search'}})">
				<image src="../../static/images/home-icon.png" class="wh36 mr-3"></image>
				<view>搜索想要找的商品</view>
			</view>
		</view>
		
		<!-- banner -->
		<container>
			<ls-swiper :list="swiperList" imgKey="imgUrl" :loop="true" :dots='true' :autoplay='true' @clickItem="clickItem()" imgRadius='5' height='160' interval='3000'/>
		</container>
		
		<view class="p-r">
			
			<view class="flexX py-3">
				<view class="i_li" :class="i_li==0?'colorM':''" @click="changeLi(0)">小学生古诗词必备80首</view>
				<view class="i_li" :class="i_li==1?'colorM':''" @click="changeLi(1)">小学一年级上</view>
				<view class="i_li" :class="i_li==2?'colorM':''" @click="changeLi(2)">小学一年级下</view>
				<view class="i_li" :class="i_li==3?'colorM':''" @click="changeLi(3)">小学二年级上</view>
				<view class="i_li" :class="i_li==4?'colorM':''" @click="changeLi(4)">小学二年级下</view>
			</view>
			<view class="f5Bj-H20"></view>
			
			<view class="line-h bB-e1 mx-3 pb-4 pt-7" v-for="(item,index) in 3" :key="index"
			@click="Router.navigateTo({route:{path:'/pages/poemsDetail/poemsDetail'}})">
				<view class="flex1 pb-3">
					<view class="font-36">尽离别·其一</view>
					<view class="font-26">清代·黄遵宪</view>
				</view>
				<view class="font-30 avoidOverflow">别肠转如轮，一刻既万周。眼见双轮驰，益增中心忧。古亦有山川，古亦有车舟。</view>
			</view>
			
		</view>
		
		
		
		
		<view style="height: 130rpx;"></view>
		<!-- footer -->
		<view class="footer">
			<view class="item on" @click="Router.redirectTo({route:{path:'/pages/index/index'}})">
				<image src="../../static/images/nabar1-a.png" mode=""></image>
				<view>首页</view>
			</view>
			<view class="item" @click="Router.redirectTo({route:{path:'/pages/ranking/ranking'}})">
				<image src="../../static/images/nabar2.png" mode=""></image>
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
	import container from '../../components/container/index.vue'
	import LsSwiper from '../../components/ls-swiper/index.vue'
	export default {
		data() {
			return {
				Router:this.$Router,
				is_show: false,
				swiperList: [{
				                type: 'image',
				                url: '../../static/images/home-banner.png'
				            }, {
				                type: 'image',
				                url: '../../static/images/home-banner.png',
				            }],
				i_li:0
			}
		},
		onLoad() {
			const self = this;
			// self.$Utils.loadAll(['getMainData'], self);
		},
		components: {
			container,
			LsSwiper
		},
		methods: {
			
			changeLi(index){
				const self = this;
				self.i_li = index;
			},
			
			getMainData() {
				const self = this;
				console.log('852369')
				const postData = {};
				postData.tokenFuncName = 'getProjectToken';
				self.$apis.orderGet(postData, callback);
			}
			
		}
	};
</script>

<style scoped>
.i_li{width: 180rpx;padding: 0 30rpx;text-align: center;flex-shrink: 0;}
.i_li:nth-child(1){width: 240rpx;}
</style>