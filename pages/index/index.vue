<template>
	<view class="container">
		<view class="banner">
			<image src="../../static/images/index/index-banner.jpg" mode="" class="bg"></image>
		</view>
		<view class="content">
			<view class="entrance">
				<view class="item">
					<image src="../../static/images/index/eat-in.png" mode="" class="icon"></image>
					<view class="title">
						堂食
					</view>
				</view>
				<view class="item">
					<image src="../../static/images/index/take-out.png" mode="" class="icon"></image>
					<view class="title">
						外卖
					</view>
				</view>
			</view>
		</view>
		<view class="info">
			<view class="integral_section">
				<view class="top">
					<view class="title">
						我的积分
					</view>
					<view class="banner">
						999
					</view>
				</view>
				<view class="bottom">
					进入积分商城兑换优惠券或周边
				</view>
			</view>
			<view class="qrcode_section">
				
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'HeHe-Shop'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang='scss' scoped>
	.container {
		.banner {
			position: relative;
			width: 100%;
			height: 480rpx;

			.bg {
				width: 100%;
				height: 480rpx;
			}
		}

		.content {
			padding: 0 32rpx;

			.entrance {
				position: relative;
				background-color: $uni-bg-color;
				border-radius: 10rpx;
				margin-top: -80rpx;
				box-shadow: $box-shadow;
				padding: 32rpx 0;
				display: flex;
				align-items: center;
				justify-content: center;

				.item {
					flex: 1;
					display: flex;
					flex-direction: column;
					align-items: center;
					position: relative;

					&:nth-child(1):after {
						content: '';
						position: absolute;
						width: 1rpx;
						background-color: #ddd;
						right: 0;
						height: 100%;
						transform: scaleX(0.5) scaleY(0.8);
					}

					.icon {
						width: 80rpx;
						height: 84rpx;
						margin-bottom: 8rpx;
					}

					.title {
						color: $uni-text-color;
					}
				}
			}
			.info{
				background-color: $uni-bg-color;
			}
		}
	}
</style>
