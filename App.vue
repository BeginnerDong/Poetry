
<script>
	import token from "./common/token.js"
	export default {
		onLaunch: function() {	
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		}
	}
</script>

<style>
	/* 富文本样式 */
	@import "/assets/style/quill.css";
	
	
	/* 公共样式 */
	@import "/common/css/common.css";
	/* 公共样式 */
	@import "/common/css/main.css";
	
	/*每个页面公共css */
	@font-face {
		font-family: 'AliM';
		src: url(https://vkceyugu.cdn.bspapp.com/VKCEYUGU-matchbox/a003f470-a6fa-11ea-a30b-e311646dfaf2.otf);
	}
	
	uni-swiper .uni-swiper-dots-horizontal{line-height: 16rpx;bottom: 5px;}
	
	uni-tabbar .uni-tabbar__icon{width: 44rpx;height: 44rpx;}
	uni-page-head .uni-page-head__title{font-weight: normal;}
	/* uni-swiper .uni-swiper-dot{width: 12rpx;height: 6rpx;border-radius: 6rpx;background-color: #c5c5c5;}
	uni-swiper .uni-swiper-dot-active{width: 20rpx;} */
	.ql-editor img{max-width: 100%;margin: 0 auto;}
	.detailBanner .uni-swiper-dots{bottom: 30rpx;}
</style>
