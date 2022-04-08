<template>
	<view>
		<view class="top"></view>
		<view class="bg"></view>
		<view class="xx"><p>分享小屋</p></view>
		<view class="dongtai" v-for="(item,i) in dt">
			<view class="user"><image :src="item[0]"><p>{{item[1]}}</p></view>
			<view class="xiaoxi">{{item[2]}}</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				xian: false,
				out:"",
					dt:[
						["../../static/icons/m1.png","清惠","苗族饰界的感受苗族是一个具有悠久的历史和深厚的文化传统的民族,是我国最古老的民族之一,人口众多,分布 辽阔。"],
						["../../static/icons/m2.png","梦瑶","上个世纪澳大利亚民族学家格迪斯在他的著述中这样感叹：“世界上有两个苦难深重而又顽强不屈的民族，他们就是中国的苗族人和分布于世界各地的犹太人。”本世纪苗族作家南往耶写道：“苗族是一个不断被驱赶甚至被消灭的民族，但他们一直没有对生命和祖先的放弃，自五千年前开始，爬山涉水，经历千难万苦，从中原逃到云贵高原和世界各地，朝着太阳落坡的地方寻找故乡，用血泪养育古歌和神话，没有怨恨，把悬崖峭壁当做家园，梯田依山而建，信仰万物，崇拜自然，祀奉祖先，感谢仇人。"],
						["../../static/icons/m3.png","嘉言","云南的风景美,云南苗族的姑娘美,能用文字描述一下吗 彩云之南山清水秀人杰地灵鸟语花香盛产好男人特产是美女楚雄苗族姑娘楚雄苗妹气质好肤白貌美大长腿。"],
						["../../static/icons/m4.png","永追随向日葵","苗族妇女上身一般穿窄袖、大领、对襟短衣,下身穿百褶裙。衣裙或长可抵足,飘逸多姿,或短不及膝,婀娜动人。便装时则多在头上包头帕,上身大襟短衣,下身长裤,镶绣花边,系一幅绣花围腰,再加少许精致银饰衬托。苗族百褶裙,图案花纹色彩斑斓,多刺绣、织锦、蜡染、挑花装饰。衣裙颜色以红、蓝、黄、白、黑为主,保持了苗族先民“三苗”“好五色衣服”的传统。"],
						["../../static/icons/m5.png","梨花薰雨","便装时则多在头上包头帕，上身大襟短衣，下身长裤，镶绣花边，系一幅绣花围腰，再加少许精致银饰衬托。"],
						["../../static/icons/m6.png","执着是爱的痛","凤凰涅槃一说出自于郭沫若先生同名作品，非中国古代传说，在中国古代神话传说中并无凤凰会浴火重生的说法。"],
						["../../static/icons/m7.png","多一度旳想念","东西收到，很满意！！真的是超级好的卖家，解答疑问不厌其烦，细致认真，关键是东西好，而且货物发得超快，包装仔细，值得信赖！"],
						["../../static/icons/m8.png","太现实的现实","我下辈子要姓夏，就叫夏课，我看那个老师敢提问我！"],
						["../../static/icons/m9.png","骨寐颜深","早上刚才收到，很是喜欢。下次还有来，介绍朋友来能不能给打个折？"]
					]
				}
		},
		methods: {
			chu(){
				this.xian = !this.xian;
			},
			toa(){
				var a = [["../../static/icons/yonghu.png","未登录",this.out]];
				this.dt = this.dt.concat(a);
				uni.showToast({
				    title: '发布成功',
				    duration: 2000
				});
				this.out = "";
				this.xian = !this.xian;
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
	.bg{
		position: fixed;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		z-index: -10;
		background: url(https://s2.loli.net/2022/03/27/xGrZVMPblE7wWOX.png);
	}
	.xx{
		width: 100%;
		height: 60rpx;
		display: flex;
		flex-direction: row;
		justify-content: center;
		align-items: center;
	}
	.xx p{
		font-size: 45rpx;
		color: #FFFFFF;
	}
	.dongtai{
		width: 100%;
	}
	.dongtai .user{
		height: 100rpx;
		display: flex;
		flex-direction: row;
		justify-content: left;
		align-items: cneter;
	}
	.dongtai .user image{
		width: 100rpx;
		height: 100rpx;
		border-radius: 50rpx;
		margin-left: 30rpx;
	}
	.dongtai .user p{
		font-size: 60rpx;
		height: 30rpx;
		margin-top: 10rpx;
	}
	.xiaoxi{
		width: 80%;
		margin: 0 auto;
	}
	.jia{
		position: fixed;
		z-index: 1000;
		right: 10rpx;
		top: 1100rpx;
		width: 100rpx;
		height: 100rpx;
		border-radius: 50rpx;
		background: #FFD700;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: cneter;
	}
	.jia p{
		margin: 0 auto;
		margin-top: -40rpx;
		width: 50rpx;
		height: 50rpx;
		font-size: 60rpx;
		text-align: center;
	}
	.shi{
		position: fixed;
		z-index: 500;
		left: 25rpx;
		top: 700rpx;
		width: 700rpx;
		height: 300rpx;
		border-radius: 30rpx;
		background: #FFD700;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: cneter;
	}
	.shuru{
		width: 600rpx;
		height:	300rpx;
		margin: 0 auto;
		margin-top: 50rpx;
		background: #C8C7CC;
	}
	.shuru textarea{
		width: 100%;
		height: 100%;
	}
	.tijiao{
		width: 140rpx;
		margin: 0 auto;
		text-align: center;
		background: red;
		border: #000000 solid 1px;
		border-radius: 5rpx;
	}
</style>

