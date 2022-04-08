<template>
	<view>
		<view class="top"></view>
		<web-view src="https://mp.weixin.qq.com/s/AcY8aWFLJzbha1Qbr_9pmg"></web-view>
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
	web-view{
		width: 100%;
		height: 100%;
	}
</style>
