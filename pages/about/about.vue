<template>
	<view class="about">
		<view class="content">
			<view style="width: 100%;align-items: center;display: flex;align-content: center;justify-content: center;">
				<image src="../../static/about.jpg" style="width: 90%;height: 400rpx;border-radius: 5rpx;"></image>
			</view>
			<view class="qrcode">

				<text class="tip">机构简介</text>
			</view>
			<view class="desc">
				<label style="font-size: 30rpx;">
				益塔机器人是吉林省蜘蛛信息技术有限公司旗下的品牌，该公司成立于2017年11月22日，是一家专注于少儿人工智能教育的科技型公司，目前在职研发人员20于人，研发的课程分二大体系，第一大体系睿智探险家针对学龄前4-5周岁的孩子，第二大体系超级工程师针对6-12周岁的孩子周岁孩子。我们的教学理念是培养孩子数学兴趣，提高孩子数学成绩。利用孩子的愿意玩和有好奇心的天性，把机器人教学和小学数学知识点有效的结合在一起，让孩子对数学产出浓厚兴趣。
			     </label>
			</view>

			
		</view>
		<!-- #ifdef APP-PLUS -->
		<view class="version">
			当前版本：{{version}}
		</view>
		<!-- #endif -->
	</view>
</template>

<script>
	export default {
		data() {
			return {
				providerList: [],
				version: '1.0',
				
			}
		},
		// #ifdef APP-PLUS
		onLoad() {
		
		},
		// #endif
		methods: {
		
		}
	}
</script>

<style>
	page,
	view {
		display: flex;
	}

	page {
		min-height: 100%;
		background-color: #FFFFFF;
	}


	.about {
		flex-direction: column;
		flex: 1;
	}

	.content {
		flex: 1;
		padding: 30upx;
		flex-direction: column;
		justify-content: center;
	}

	.qrcode {
		display: flex;
		align-items: center;
		flex-direction: column;
	}

	.qrcode .tip {
		margin-top: 20upx;
		font-size: 35rpx;
	}

	.desc {
		margin-top: 30upx;
		display: block;
	}

	.code {
		color: #e96900;
		background-color: #f8f8f8;
	}

	button {
		width: 100%;
		margin-top: 40upx;
	}

	.version {
		height: 80upx;
		line-height: 80upx;
		justify-content: center;
		color: #ccc;
	}

	.source {
		margin-top: 30upx;
		flex-direction: column;
	}

	.source-list {
		flex-direction: column;
	}

	.link {
		color: #007AFF;
	}
</style>
