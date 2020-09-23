<template>
	<view>
		
		<image src="../../static/images/img1.png" mode="widthFix" class="bgImg"></image>
		
		<view class="p-r px-3">
			
			<view class="bB-e1">
				<view class="font-34 line-h pt-4">姓名</view>
				<input type="text" value="张丹" placeholder="请输入姓名" />
			</view>
			<view class="bB-e1">
				<view class="font-34 line-h pt-4">电话</view>
				<input type="text" value="15682395740" placeholder="请输入姓名" />
			</view>
			<view class="bB-e1">
				<view class="font-34 line-h pt-4">身份证号</view>
				<input type="text" value="40125856848755845" placeholder="请输入姓名" />
			</view>
			
			<!-- 班主任、老师 -->
			<picker mode="selector">
				<view class="bB-e1">
					<view class="font-34 line-h pt-4">类型</view>
					<view class="txt">班主任</view>
				</view>
			</picker>
			<picker mode="selector">
				<view class="bB-e1">
					<view class="font-34 line-h pt-4">省份</view>
					<view class="txt">广东省</view>
				</view>
			</picker>
			<picker mode="selector">
				<view class="bB-e1">
					<view class="font-34 line-h pt-4">地级市</view>
					<view class="txt">广东省</view>
				</view>
			</picker>
			<picker mode="selector">
				<view class="bB-e1">
					<view class="font-34 line-h pt-4">市县</view>
					<view class="txt">广东省</view>
				</view>
			</picker>
			<picker mode="selector">
				<view class="bB-e1">
					<view class="font-34 line-h pt-4">学校名称</view>
					<view class="txt">新蕾幼儿园</view>
				</view>
			</picker>
			<view class="bB-e1">
				<view class="font-34 line-h pt-4">学校地址</view>
				<input type="text" value="宝安区保安六十五区" placeholder="请输入学校地址" />
			</view>
			<view class="bB-e1">
				<view class="font-34 line-h pt-4">班级名称</view>
				<input type="text" value="大一班" placeholder="请输入班级名称" />
			</view>
			
			<!-- 家长、学生 -->
			<picker mode="selector">
				<view class="bB-e1">
					<view class="font-34 line-h pt-4">入学年份</view>
					<view class="txt">2017</view>
				</view>
			</picker>
			<view class="bB-e1">
				<view class="font-34 line-h pt-4">学号</view>
				<input type="text" value="2255115" placeholder="请输入学号" />
			</view>
			<view class="bB-e1">
				<view class="font-34 line-h pt-4">学生身份证</view>
				<input type="text" value="152695426958" placeholder="请输入学生身份证" />
			</view>
			<view class="bB-e1">
				<view class="font-34 line-h pt-4">学生手机号</view>
				<input type="text" value="152695426958" placeholder="请输入学生手机号" />
			</view>
			<view class="bB-e1">
				<view class="font-34 line-h pt-4">监护人姓名</view>
				<input type="text" value="152695426958" placeholder="请输入监护人姓名" />
			</view>
			<view class="bB-e1">
				<view class="font-34 line-h pt-4">监护人微信号</view>
				<input type="text" value="152695426958" placeholder="请输入监护人微信号" />
			</view>
			<picker mode="selector">
				<view class="bB-e1">
					<view class="font-34 line-h pt-4">亲属关系</view>
					<view class="txt">爸爸</view>
				</view>
			</picker>
			<view class="bB-e1">
				<view class="font-34 line-h pt-4">家庭住址</view>
				<input type="text" value="152695426958" placeholder="请输入家庭住址" />
			</view>
			<view class="bB-e1">
				<view class="font-34 line-h pt-4">班主任</view>
				<input type="text" value="152695426958" placeholder="请输入班主任姓名" />
			</view>
			<view class="bB-e1">
				<view class="font-34 line-h pt-4">班主任手机号</view>
				<input type="text" value="152695426958" placeholder="请输入班主任手机号" />
			</view>
			<view class="bB-e1">
				<view class="font-34 line-h pt-4">班主任微信号</view>
				<input type="text" value="152695426958" placeholder="请输入班主任微信号" />
			</view>
			
			
			
			
			<view class="font-32 p-r btn"
			@click="Router.navigateTo({route:{path:'/pages/poemsDetail/poemsDetail?type=1'}})">
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
				Router:this.$Router
			}
		},
		methods: {
			
		}
	}
</script>

<style scoped>
input,.txt{font-size: 30rpx;height: 88rpx;line-height: 88rpx;}
.btn{margin-top: 100rpx;margin-bottom: 100rpx;}
</style>
