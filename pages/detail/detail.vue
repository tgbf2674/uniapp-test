<template>
	<view class="content">
		<view class="swiper-container">
			<swiper :indicator-dots="true" :autoplay="true" :interval="3000" :duration="1000">
				<swiper-item>
					<view class="swiper-item uni-badge-green">
						<image src="../../static/logo.png" mode=""></image>
					</view>
				</swiper-item>
				<swiper-item>
					<view class="swiper-item uni-badge-danger">
						<image src="../../static/logo.png" mode=""></image>
					</view>
				</swiper-item>
			</swiper>
		</view>
		<view class="textcont">
			<text class="title">happy birthday to u</text>
			<view>
			<text style="font-size: 14px;">xxxxx</text>
			</view>
			<view class="price">
			<text>$31.8</text>
			</view>
			<view class="desc">
				<view>/xxxx/</view>
				<view>/xxxx/</view>
				<view>/xxxx/</view>
			</view>
		</view>
		<view class="imgs">
			<image src="../../static/logo.png" mode=""></image>
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

<style lang="scss" scoped>
	.content{
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
		.swiper-container {
			width: 100%;
			text-align: center;
		}
		.textcont{
			.title{
				font-weight: normal;
				font-size: 50rpx;
			}
			.price{
				font-size: 44rpx;
				color: #c69c6d;
			}
			.desc{
				width: 100%;
				text-align: left;
			}
		}
		
	}
</style>
