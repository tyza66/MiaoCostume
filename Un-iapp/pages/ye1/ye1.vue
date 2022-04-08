<template>
	<view>
		<view class="top"></view>
		<web-view src="https://mp.weixin.qq.com/s/fnKi4IJr0RAQT-6mmT9PxQ"></web-view>
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
