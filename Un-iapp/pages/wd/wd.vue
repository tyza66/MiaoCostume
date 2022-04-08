<template>
	<view>
		<view class="top"></view>
		<view class="back"></view>
		<view class="bg"></view>
		<view class="name">
			<image src="../../static/icons/yonghu.png"></image>
			<p class="p1">未登录</p>
			<p class="p2"><u>微信登陆</u></p>
			<p class="p3"><u>手机注册</u></p>
		</view>
		<view class="items">
			<view class="item">
				<view class="one">
					<image src="../../static/icons/l1.png"></image>
					<p>礼品</p>
				</view>
				<view class="one">
					<image src="../../static/icons/l2.png"></image>
					<p>优惠券</p>
				</view>
				<view class="one">
					<image src="../../static/icons/l3.png"></image>
					<p>信息</p>
				</view>
				<view class="one">
					<image src="../../static/icons/l4.png"></image>
					<p>红包</p>
				</view>
			</view>
			<view class="item">
				<view class="one">
					<image src="../../static/icons/l5.png"></image>
					<p>应用中心</p>
				</view>
				<view class="one">
					<image src="../../static/icons/l6.png"></image>
					<p>攻略</p>
				</view>
				<view class="one">
					<image src="../../static/icons/l7.png"></image>
					<p>话题</p>
				</view>
				<view class="one">
					<image src="../../static/icons/l8.png"></image>
					<p>发现</p>
				</view>
			</view>
			<view class="sp">
				<view class="sc">
					<view class="pp1"><p>·我的收藏</p></view>
					<view class="pp2">
						<image src="https://s2.loli.net/2022/03/27/aqejWF4725ZouM9.png"></image>
						<image src="https://s2.loli.net/2022/03/27/Xr8GWiouYQ6jk3C.png"></image>
						<image src="https://s2.loli.net/2022/03/27/Khp32dCJe4uXj6Q.png"></image>
						<image src="https://s2.loli.net/2022/03/27/DEvz1hPyjQJKl9p.png"></image>
						<image src="https://s2.loli.net/2022/03/27/qpV7UzSvZXhw3cu.png"></image>
					</view>
				</view>
				<view class="gm">
					<view class="pp1"><p>·购买记录</p></view>
					<view class="pp2">
						<image src="https://s2.loli.net/2022/03/27/aqejWF4725ZouM9.png"></image>
						<image src="https://s2.loli.net/2022/03/27/Xr8GWiouYQ6jk3C.png"></image>
						<image src="https://s2.loli.net/2022/03/27/Khp32dCJe4uXj6Q.png"></image>
						<image src="https://s2.loli.net/2022/03/27/DEvz1hPyjQJKl9p.png"></image>
						<image src="https://s2.loli.net/2022/03/27/qpV7UzSvZXhw3cu.png"></image>
					</view>
				</view>
				<view class="qb">
					<view class="pp1"><p>·我的钱包</p></view>
					<view class="pp2">
						<p>我的平台钱包：余额￥2000</p>
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
				
			}
		},
		methods: {
			
		}
	}
</script>

<style>
	.top {
		height: var(--status-bar-height);
		width: 100%;
		background-color: #FFFFFF;
	}
	.back{
		position: fixed;
		width: 100%;
		height: 100%;
		background: rgba(4,249,7,0.3);
	}
	.bg{
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 400rpx;
		background: linear-gradient(#E75603, pink);
	}
	.name{
		position: absolute;
		width: 100%;
		height: 200rpx;
		top: 120rpx;
	}
	.name image{
		width: 150rpx;
		height: 150rpx;
		border-radius: 75rpx;
		margin-top: 30rpx;
		margin-left: 30rpx;
	}
	.p1{
		color: #FFFFFF;
		font-size: 30rpx;
		position: absolute;
		top: 50rpx;
		left: 200rpx;
	}
	.p2{
		color: #FFFFFF;
		font-size: 30rpx;
		position: absolute;
		top: 120rpx;
		left: 200rpx;
	}
	.p3{
		color: #FFFFFF;
		font-size: 30rpx;
		position: absolute;
		top: 120rpx;
		left: 350rpx;
	}
	.items{
		position: absolute;
		width: 100%;
		top: 400rpx;
	}
	.item{
		position: relative;
		float: left;
		width: 100%;
		height: 150rpx;
		background: #FFFFFF;
		border-radius: 25rpx;
		margin-bottom: 35rpx;
		margin-top: -25rpx;
		display: flex;
		flex-direction: row;
		justify-content: center;
		align-items: center;
	}
	.one{
		width: 120rpx;
		height: 130rpx;
		margin: 0 auto;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}
	.one image{
		width: 60rpx;
		height: 60rpx;
	}
	.one p{
		font-size: 30rpx;
	}
	.sp{
		height: 500rpx;
		position: relative;
		width: 100%;
		background: #FFFFFF;
		border-radius: 25rpx;
		margin-top: -25rpx;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}
	.sc{
		width: 95%;
		height: 150rpx;
	}
	.gm{
		width: 95%;
		height: 150rpx;
	}
	.qb{
		width: 95%;
		height: 150rpx;
	}
	.pp1{
		width: 100%;
		height: 60rpx;
		display: flex;
		flex-direction: row;
		justify-content: left;
		align-items: center;
	}
	.pp1{
		font-family: "幼圆";
	}
	.pp2{
		width: 100%;
		height: 90rpx;
		display: flex;
		flex-direction: row;
		justify-content: ceter;
		align-items: center;
	}
	.pp2 image{
		width: 90rpx;
		height: 90rpx;
		margin: 0 auto;
	}
</style>
