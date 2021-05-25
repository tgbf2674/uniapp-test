<template>
	<view class="content">
		<view class="topbar">
			<image src="../../static/logo.png" mode=""></image>
		</view>
		<view class="fill"></view>
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
		<view class="uni-flex uni-row fontsize">
			<view class="flex-item ">新客满298元赠送切块蛋糕</view>
			<view class="flex-item " style="margin: 0 10rpx;">满100元包邮</view>
			<view class="flex-item ">全程冷链配送</view>
		</view>
		<view class="uni-flex uni-row ico">
			<view class="flex-item ">
				<image src="../../static/logo.png" mode="">蛋糕</image>
			</view>
			<view class="flex-item ">
				<image src="../../static/logo.png" mode="">蛋糕</image>
			</view>
			<view class="flex-item ">
				<image src="../../static/logo.png" mode="">蛋糕</image>
			</view>
			<view class="flex-item ">
				<image src="../../static/logo.png" mode="">蛋糕</image>
			</view>
		</view>
		<view class="goods">
			<view class="list">
				<view class="cover">
					<image src="../../static/logo.png" mode=""></image>
				</view>
				<view class="text">
					<view class="cart"></view>
					<view>
						<text class="name">别人的（HBD）</text>
						<text class="price">198</text>
						<text class="size">/元454g</text>
					</view>
					<view class="des">
						<text>猪年限定款</text>
					</view>
				</view>
			</view>
			<view class="list">
				<view class="cover">
					<image src="../../static/logo.png" mode=""></image>
				</view>
				<view class="text">
					<view>
						<text class="name">别人的（HBD）</text>
						<text class="price">198</text>
						<text class="size">/元454g</text>
					</view>
					<view class="des">
						<text>猪年限定款</text>
					</view>
				</view>
			</view>
			<view class="list">
				<view class="cover">
					<image src="../../static/logo.png" mode=""></image>
				</view>
				<view class="text">
					<view>
						<text class="name">别人的（HBD）</text>
						<text class="price">198</text>
						<text class="size">/元454g</text>
					</view>
					<view class="des">
						<text>猪年限定款</text>
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
				title: 'Hello'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang="scss" scoped>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;

		.topbar {
			position: fixed;
			top: 0;
			left: 0;
			width: 100%;
			background: #FFFFFF;
			height: 48*2rpx;
			box-shadow: 0px 2px 4px 0px rgba(0, 0, 0, 0.1);
			text-align: center;

			image {
				width: 60rpx;
				height: 60rpx;
				margin: 20rpx;
			}
		}

		.fill {
			width: 100%;
			height: 96rpx;
		}

		.swiper-container {
			width: 100%;
			height: 440rpx;
			border: 1px solid red;
			text-align: center;
		}
		.fontsize{
			font-size: 28rpx;
		}
		.ico{
			text-align: center;
			image{
				width: 58*2rpx;
				height: 58*2rpx;
				display: block;
				padding: 0 12*2rpx;
			}
		}
		.goods{
			width: 90%;
			border-top: 1px solid #B2B2B2;
			margin-top: 20rpx;
			.list{
				margin: 50rpx 0;
				box-shadow: 0 4px 4px 0 #BBBBBB;
				border-radius: 4px;
				.cover{
					width: 100%;
					height: 396rpx;
					image{
						width: 100%;
						height: 100%;
					}
				}
				.text{
					padding: 20px 0 0 10rpx;
					.cart{
						width: 60rpx;
						height: 60rpx;
						float: right;
						margin: 10rpx 20rpx 0 0;
						border-radius: 50%;
						box-shadow: 0 2px 4px 0 rgba(0,0,0,0.1);
						background:url(../../static/logo.png) no-repeat;
						background-position: -90rpx -10rpx;
						background-size: 160rpx auto;
					}
					.name{
						font-weight: bold;
						font-size: 15px;
						color: #322418;
					}
					.price{
						color: #c69c6d;
						margin-left: 10px;
					}
					.size{
						color: #B2B2B2;
					}
					.des{
						color: #442818;
					}
				}
			}
		}
	}
</style>
