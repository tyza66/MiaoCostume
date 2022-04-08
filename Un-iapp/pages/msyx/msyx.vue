<template>
	<view>
		<view class="top"></view>
		<view class="mianfei"><image src="../../static/icons/logo.png"></image></view>
		<view class="ss">
			<view class="kuang"><input type="text" v-model="index1"><image src="../../static/icons/ss.png" @click="search()"></view>
		</view>
		<view class="mainfei1">
			<view class="one" v-show="a1">
				<view class="im"><image src="https://s2.loli.net/2022/03/27/zcgqwN85FpALbDV.png"></image></view>
				<view class="ti"><p>定制银手镯</p></view>
				<view class="up"><p>售价：￥499</p><image src="../../static/icons/xi.png" v-if="!z1" @click="zan(z1)"><image src="../../static/icons/xi2.png"  v-if="z1" @click="zan(z1)"></view>
			</view>
			<view class="one" v-show="a2">
				<view class="im"><image src="https://s2.loli.net/2022/03/27/VLqtOkGvWcmafNQ.png"></image></view>
				<view class="ti"><p>蝴蝶耳饰</p></view>
				<view class="up"><p>售价：￥299</p><image src="../../static/icons/xi.png" v-if="!z2" @click="zan(z2)"><image src="../../static/icons/xi2.png"  v-if="z2" @click="zan(z2)"></view>
			</view>
			<view class="one" v-show="a3">
				<view class="im"><image src="https://s2.loli.net/2022/03/27/aqejWF4725ZouM9.png"></image></view>
				<view class="ti"><p>特色银饰</p></view>
				<view class="up"><p>售价：￥1299</p><image src="../../static/icons/xi.png" v-if="!z3" @click="zan(z3)"><image src="../../static/icons/xi2.png"  v-if="z3" @click="zan(z3)"></view>
			</view>
			<view class="one" v-show="a4">
				<view class="im"><image src="https://s2.loli.net/2022/03/27/Xr8GWiouYQ6jk3C.png"></image></view>
				<view class="ti"><p>蝴蝶戒指</p></view>
				<view class="up"><p>售价：￥399</p><image src="../../static/icons/xi.png" v-if="!z4" @click="zan(z4)"><image src="../../static/icons/xi2.png"  v-if="z4" @click="zan(z4)"></view>
			</view>
			<view class="one" v-show="a5">
				<view class="im"><image src="https://s2.loli.net/2022/03/27/yNlwHufxWkj4mqX.png"></image></view>
				<view class="ti"><p>苗族银耳环</p></view>
				<view class="up"><p>售价：￥199</p><image src="../../static/icons/xi.png" v-if="!z5" @click="zan(z5)"><image src="../../static/icons/xi2.png"  v-if="z5" @click="zan(z5)"></view>
			</view>
			<view class="one" v-show="a6">
				<view class="im"><image src="https://s2.loli.net/2022/03/27/abm284xQ9iNUJwe.png"></image></view>
				<view class="ti"><p>侗族头饰</p></view>
				<view class="up"><p>售价：￥99</p><image src="../../static/icons/xi.png" v-if="!z6" @click="zan(z6)"><image src="../../static/icons/xi2.png"  v-if="z6" @click="zan(z6)"></view>
			</view>
			<view class="one" v-show="a7">
				<view class="im"><image src="https://s2.loli.net/2022/03/27/jLxZfRa2JFmUPpl.png"></image></view>
				<view class="ti"><p>手工银耳环</p></view>
				<view class="up"><p>售价：￥300</p><image src="../../static/icons/xi.png" v-if="!z7" @click="zan(z7)"><image src="../../static/icons/xi2.png"  v-if="z7" @click="zan(z7)"></view>
			</view>
			<view class="one" v-show="a8">
				<view class="im"><image src="https://s2.loli.net/2022/03/27/Khp32dCJe4uXj6Q.png"></image></view>
				<view class="ti"><p>流苏耳串</p></view>
				<view class="up"><p>售价：￥400</p><image src="../../static/icons/xi.png" v-if="!z8" @click="zan(z8)"><image src="../../static/icons/xi2.png"  v-if="z8" @click="zan(z8)"></view>
			</view>
			<view class="one" v-show="a9">
				<view class="im"><image src="https://s2.loli.net/2022/03/27/qEQxdOjc5Z6HM2u.png"></image></view>
				<view class="ti"><p>苗族银项圈</p></view>
				<view class="up"><p>售价：￥600</p><image src="../../static/icons/xi.png" v-if="!z9" @click="zan(z9)"><image src="../../static/icons/xi2.png"  v-if="z9" @click="zan(z9)"></view>
			</view>
			<view class="one" v-show="a10">
				<view class="im"><image src="https://s2.loli.net/2022/03/27/DEvz1hPyjQJKl9p.png"></image></view>
				<view class="ti"><p>苗族项圈</p></view>
				<view class="up"><p>售价：￥600</p><image src="../../static/icons/xi.png" v-if="!z10" @click="zan(z10)"><image src="../../static/icons/xi2.png"  v-if="z10" @click="zan(z10)"></view>
			</view>
			<view class="one" v-show="a11">
				<view class="im"><image src="https://s2.loli.net/2022/03/27/qpV7UzSvZXhw3cu.png"></image></view>
				<view class="ti"><p>铃铛手镯</p></view>
				<view class="up"><p>售价：￥300</p><image src="../../static/icons/xi.png" v-if="!z11" @click="zan(z11)"><image src="../../static/icons/xi2.png"  v-if="z11" @click="zan(z11)"></view>
			</view>
			<view class="one" v-show="a12">
				<view class="im"><image src="https://s2.loli.net/2022/03/27/auJV8YyInl4jmwE.png"></image></view>
				<view class="ti"><p>苗族宽手镯</p></view>
				<view class="up"><p>售价：￥599</p><image src="../../static/icons/xi.png" v-if="!z12" @click="zan(z12)"><image src="../../static/icons/xi2.png"  v-if="z12" @click="zan(z12)"></view>
			</view>
			<view class="one" v-show="a13">
				<view class="im"><image src="https://s2.loli.net/2022/03/27/fY6mnuZ8lgUKdBw.png"></image></view>
				<view class="ti"><p>个性戒指</p></view>
				<view class="up"><p>售价：￥100</p><image src="../../static/icons/xi.png" v-if="!z13" @click="zan(z13)"><image src="../../static/icons/xi2.png"  v-if="z13" @click="zan(z13)"></view>
			</view>
			<view class="one" v-show="a14">
				<view class="im"><image src="https://s2.loli.net/2022/03/27/Cnsi1APzh3BOwQ9.png"></image></view>
				<view class="ti"><p>苗族头饰</p></view>
				<view class="up"><p>售价：￥9000</p><image src="../../static/icons/xi.png" v-if="!z14" @click="zan(z14)"><image src="../../static/icons/xi2.png"  v-if="z14" @click="zan(z14)"></view>
			</view>
			<view class="one" v-show="a15">
				<view class="im"><image src="https://s2.loli.net/2022/03/27/GyznCp1FschlrkV.png"></image></view>
				<view class="ti"><p>苗族手镯</p></view>
				<view class="up"><p>售价：￥200</p><image src="../../static/icons/xi.png" v-if="!z15" @click="zan(z15)"><image src="../../static/icons/xi2.png"  v-if="z15" @click="zan(z15)"></view>
			</view>
			<view class="one" v-show="a16">
				<view class="im"><image src="https://s2.loli.net/2022/03/27/Jg3EcuOXhTtNA9Q.png"></image></view>
				<view class="ti"><p>凯里耳环</p></view>
				<view class="up"><p>售价：￥199</p><image src="../../static/icons/xi.png" v-if="!z16" @click="zan(z16)"><image src="../../static/icons/xi2.png"  v-if="z16" @click="zan(z16)"></view>
			</view>
			<view class="one" v-show="a17">
				<view class="im"><image src="https://s2.loli.net/2022/03/27/vadzJtinolfmTMU.png"></image></view>
				<view class="ti"><p>牛角头饰</p></view>
				<view class="up"><p>售价：￥999</p><image src="../../static/icons/xi.png" v-if="!z17" @click="zan(z17)"><image src="../../static/icons/xi2.png"  v-if="z17" @click="zan(z17)"></view>
			</view>
			<view class="one" v-show="a18">
				<view class="im"><image src="https://s2.loli.net/2022/03/27/a4rO6o5MSENePpG.png"></image></view>
				<view class="ti"><p>演出饰品</p></view>
				<view class="up"><p>售价：￥50</p><image src="../../static/icons/xi.png" v-if="!z18" @click="zan(z18)"><image src="../../static/icons/xi2.png"  v-if="z18" @click="zan(z18)"></view>
			</view>
			<view class="one" v-show="a19">
				<view class="im"><image src="https://s2.loli.net/2022/03/27/GQgswiEC9mzXK7D.png"></image></view>
				<view class="ti"><p>演出头饰</p></view>
				<view class="up"><p>售价：￥60</p><image src="../../static/icons/xi.png" v-if="!z19" @click="zan(z19)"><image src="../../static/icons/xi2.png"  v-if="z19" @click="zan(z19)"></view>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				a1: true,
				a2: true,
				a3: true,
				a4: true,
				a5: true,
				a6: true,
				a7: true,
				a8: true,
				a9: true,
				a10: true,
				a12: true,
				a13: true,
				a14: true,
				a15: true,
				a16: true,
				a17: true,
				a18: true,
				a19: true,
				index1: "",
				z1: false,
				z2: false,
				z3: false,
				z4: false,
				z5: false,
				z6: false,
				z7: false,
				z8: false,
				z9: false,
				z10: false,
				z11: false,
				z12: false,
				z13: false,
				z14: false,
				z15: false,
				z16: false,
				z17: false,
				z18: false,
				z19: false
			}
		},
		onLoad() {

		},
		methods: {
			zan(ina){
				console.log(ina);
				ina = !ina;
			},
			clear(){
				this.a1 = false;
				this.a2 = false;
				this.a3 = false;
				this.a4 = false;
				this.a5 = false;
				this.a6 = false;
				this.a7 = false;
				this.a8 = false;
				this.a9 = false;
				this.a10 = false;
				this.a11 = false;
				this.a12 = false;
				this.a13 = false;
				this.a14 = false;
				this.a15 = false;
				this.a16 = false;
				this.a17 = false;
				this.a18 = false;
				this.a19 = false;
			},
			all(){
				this.a1 = true;
				this.a2 = true;
				this.a3 = true;
				this.a4 = true;
				this.a5 = true;
				this.a6 = true;
				this.a7 = true;
				this.a8 = true;
				this.a9 = true;
				this.a10 = true;
				this.a11 = true;
				this.a12 = true;
				this.a13 = true;
				this.a14 = true;
				this.a15 = true;
				this.a16 = true;
				this.a17 = true;
				this.a18 = true;
				this.a19 = true;
			},
			search(){
				if(this.index1==""){
					this.all();
				}
				else if(this.index1=="手镯"){
					this.clear();
					this.a1 = true;
					this.a11 = true;
					this.a12 = true;
				}
				else if(this.index1=="头饰"){
					this.clear();
					this.a6 = true;
					this.a14 = true;
					this.a18 = true;
					this.a19 = true;
				}
				else if(this.index1=="耳环"){
					this.clear();
					this.a2 = true;
					this.a5 = true;
					this.a7 = true;
					this.a8 = true;
					this.a16 = true;
				}
				else if(this.index1=="戒指"){
					this.clear();
					this.a4 = true;
					this.a13 = true;
				}
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
	.mianfei{
		width: 100%;
		height: 120rpx;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}
	.ss{
		width: 100%;
		height: 60rpx;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}
	.kuang{
		width: 80%;
		height: 95%;
		background: #C8C7CC;
		border-radius: 15rpx;
		display: flex;
		flex-direction: row;
		justify-content: center;
		align-items: center;
	}
	.kuang input{
		width: 85%;
		height: 100%;
	}
	.kuang image{
		width: 50rpx;
		height: 50rpx;
	}
	.mianfei se-image{
		width: 80%;
		height: 100%;
	}
	.one{
		float: left;
		height: 340rpx;
		width: 49%;
		margin-left: 1%;
		margin-top: 10rpx;
		border-radius: 10rpx;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		background: #F8F8F8;
	}
	.one .im{
		width: 100%;
		height: 60%;
	}
	.one .im image{
		width: 100%;
		height: 100%;
	}
	.one .ti{
		width: 100%;
		height: 20%;
	}
	.one .ti p{
		text-align: center;
		width: 100%;
		height: 20%;
	}
	.one .up{
		width: 100%;
		height: 20%;
		display: flex;
		flex-direction: row;
		justify-content: left;
		align-items: center;
	}
	.up image{
		width: 30rpx;
		height: 30rpx;
		margin-left: 10rpx;
	}
</style>
