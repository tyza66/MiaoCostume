<template>
	<view class="content">
		<view class="top"></view>
		<view class="swiper-c">
			<swiper indicator-dots="true" autoplay="autoplay" interval="1000" duration="500">
				<swiper-item>
					<image src="../../static/picture/sheji1.png"></image>
				</swiper-item>
				<swiper-item>
					<image src="../../static/picture/sheji2.png"></image>
				</swiper-item>
				<swiper-item>
					<image src="../../static/picture/sheji3.png"></image>
				</swiper-item>
				<swiper-item>
					<image src="../../static/picture/g4.png"></image>
				</swiper-item>
			</swiper>
		</view>
		<view class="swiper-c2">
			<swiper vertical="true" autoplay="autoplay" interval="1500" duration="500">
				<swiper-item>
					<view>
						<p class="a1">公众号</p>
						<p class="a2">关注苗族饰界微信公众号，最快速获得相关咨询...</p>
					</view>
					<view>
						<p class="a1">文章</p>
						<p class="a2">将中国传统的非物质文化遗产，以一种独特的...</p>
					</view>
				</swiper-item>
				<swiper-item>
					<view>
						<p class="a1">文章</p>
						<p class="a2">饰界伊始：热馨护工竞选比赛正在进行，快进来...</p>
					</view>
					<view>
						<p class="a1">文章</p>
						<p class="a2">苗族银饰 一次偶遇：苗族银饰作为一种文化现象...</p>
					</view>
				</swiper-item>
			</swiper>
		</view>
		<view class="tj">
			<view @click="p1()"><image src="../../static/picture/pi12.png"></image></view>
			<view @click="p2()"><image src="../../static/picture/pi13.png"></image></view>
		</view>
		<view class="tuijian">
			<view class="tit"><p>动态</p></view> 
			<view class="b1">
				<view class="p1"><p>·最新动态</p></view>
				<view class="p2"><image src="../../static/icons/shangbiao.png"></image><p>新品发布！可定制手镯风格！</p></view>
				<view class="p2"><image src="../../static/icons/shangbiao2.png"></image><p>我们的公众号开通啦！</p></view>
				<view class="p2"><image src="../../static/icons/shangbiao.png"></image><p>新季度上新货！低库存可速入收藏！</p></view>
			</view>
			<view class="b1">
				<view class="p1"><p>·介绍产品</p></view>
				<view class="p2"><image src="../../static/icons/shangbiao2.png"></image><p>我们的品牌！苗族饰界！</p></view>
				<view class="p2"><image src="../../static/icons/shangbiao.png"></image><p>苗族将蝴蝶妈妈作为图腾之一...</p></view>
				<view class="p2"><image src="../../static/icons/shangbiao2.png"></image><p>意在打造你的第一款时尚艺术收藏...</p></view>
			</view>
			<view class="b1">
				<view class="p1"><p>·VI设计</p></view>
				<view class="p2"><image src="../../static/icons/shangbiao.png"></image><p>公司愿景是通过打造自己的品牌计...</p></view>
				<view class="p2"><image src="../../static/icons/shangbiao2.png"></image><p>苗族饰界意在打造中国文艺收藏品...</p></view>
				<view class="p2"><image src="../../static/icons/shangbiao.png"></image><p>有非遗传承人龙太阳先生和潘仕学...</p></view>
			</view>
			<view class="b1">
				<view class="p1"><p>·品牌信息</p></view>
				<view class="p2"><image src="../../static/icons/shangbiao2.png"></image><p>苗族的视觉元素主要体现在旁边的...</p></view>
				<view class="p2"><image src="../../static/icons/shangbiao.png"></image><p>达到传承非遗技艺，弘扬国朝文化...</p></view>
				<view class="p2"><image src="../../static/icons/shangbiao2.png"></image><p>时尚消费品（推出首款品牌产品...</p></view>
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
		onLoad() {

		},
		methods: {
			p1(){
				uni.navigateTo({
					url:"../ye1/ye1"
				});
			},
			p2(){
				uni.navigateTo({
					url:"../ye2/ye2"
				});
			}
		}
	}
</script>

<style>
	.top {
		height: var(--status-bar-height);
		width: 100%;
		background-color: #FFFFFF;
	}
	.swiper-c{
		width: 100%;
		height: 450rpx;
	}
	.swiper-c swiper{
		width: 100%;
		height: 100%;
	}
	.swiper-c swiper swiper-item image{
		width: 100%;
		height: 100%;
	}
	.swiper-c2{
		width: 90%;
		height: 100rpx;
		margin: 0 auto;
	}
	.swiper-c2 swiper{
		width: 100%;
		height: 100%;
	}
	.swiper-c2 swiper swiper-item view{
		height: 50%;
		display: flex;
		flex-direction: row;
		align-items: center;
	}
	.tj{
		width: 100%;
		margin: 0 auto;
	}
	.tj view{
		margin: 0 auto;
		width: 95%;
	}
	.tj view image{
		width: 100%;
		margin: 0 auto;
	}
	.a1{
		font-size: 15rpx;
		text-align: center;
		color: #DD524D;
		width: 85rpx;
		height: 65%;
		border: #DD524D solid 1px;
		border-radius: 15rpx;
		margin-left: 20rpx;
	}
	.a2{
		margin-left: 10rpx;
		text-align: center;
		font-size: 15rpx;
	}
	.tuijian{
		width: 90%;
		margin: 0 auto;
		border-radius: 15rpx;
		margin-top: 10rpx;
	}
	.tit{
		height: 80rpx;
		width: 100%;
		display: flex;
		flex-direction: row;
		justify-content: left;
		align-items: center;
	}
	.tit p{
		font-family: "幼圆";
		font-weight: 600;
		font-size: 45rpx;
		margin-left: 15rpx;
	}
	.b1{
		width: 600rpx;
		height: 300rpx;
		margin: 0 auto;
		margin-top: 5rpx;
		border-radius: 15rpx;
	}
	.p1{
		width: 100%;
		height: 60rpx;

		display: flex;
		flex-direction: row;
		justify-content: left;
		align-items: center;
	}
	.p1 p{
		font-family: "幼圆";
	}
	.p2{
		width: 100%;
		height: 80rpx;

		display: flex;
		flex-direction: row;
		justify-content: left;
		align-items: center;
	}
	.p2 image{
		width: 80rpx;
		height: 80rpx;
	}
	.p2 p{
		
	}
</style>
