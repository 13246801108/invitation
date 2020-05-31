<template>
	<view class="openPage">
		<view class="open_animation flex flex-center">
			<image src="../../assets/imgs/open_bg.png" mode="aspectFit" class="open_bg "></image>
		</view>
		<view class="open_content">
			<slot></slot>
		</view>
	</view>
</template>

<script>
</script>

<style>
	.openPage{
		width: 100%;
		height: 100%;
		position: relative;
	}
	.openPage .open_content{
		position: absolute;
		top: 0;
		left: 0;
		bottom: 0;
		right: 0;
		z-index: 2;
	}
	.openPage .open_animation{
		position: absolute;
		top: 0;
		left: 0;
		bottom: 0;
		right: 0;
	}
	.openPage .open_bg{
		width: 100%;
		height: 100%;
		/* padding: 30upx; */
	}
</style>
