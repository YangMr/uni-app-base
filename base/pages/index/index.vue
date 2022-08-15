<template>
	<view class="content">
		<!--#ifdef H5 -->
		<view>积云教育</view>
		<!-- #endif -->
		
		<!-- #ifdef APP-PLUS -->
		<view>积云教育APP</view>
		<!-- #endif -->
		
		<!-- #ifdef MP-WEIXIN -->
		<view>积云教育小程序</view>
		<!-- #endif -->
		
		<!-- #ifndef MP-WEIXIN || H5 -->
		<view>2108A百分百就业</view>
		<!-- #endif -->
		
		<view>
			{{title}}
		</view>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				// #ifdef H5
				title: 'Hello 积云 h5',
				// #endif
				// #ifdef APP-PLUS
				title: 'Hello 积云 App',
				// #endif
				// #ifdef MP-WEIXIN
				title: 'Hello 积云 小程序',
				// #endif
			}
		},
		onLoad() {
			
		},
		methods: {

		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
</style>
