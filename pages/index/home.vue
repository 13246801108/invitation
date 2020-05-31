<template>
	<view class="container">
		<swiper :duration="1000" :vertical="true" class="invite_swiper" :circular="true">
			<swiper-item>
				<openBg>
					<page1></page1>
				</openBg>
			</swiper-item>
			<swiper-item>
				<openBg>
					<page2></page2>
				</openBg>
			</swiper-item>
			<swiper-item>
				<openBg>
					<page3></page3>
				</openBg>
			</swiper-item>
			<swiper-item>
				<openBg>
					<page4></page4>
				</openBg>
			</swiper-item>
		</swiper>
	</view>
</template>

<script>
	import page1 from "pages/index/comPage1.vue";
	import page2 from "pages/index/comPage2.vue";
	import page3 from "pages/index/comPage3.vue";
	import page4 from "pages/index/comPage4.vue";
	import openBg from "pages/index/comOpen.vue";
	export default {
		data() {
			return {
			}
		},
		onLoad() {

		},
		watch:{
		},
		components:{page1,page2,page3,page4,openBg},
		methods: {
			jump(url){
				console.log(url);
				uni.navigateTo({url});
			}
		}
	}
</script>

<style scoped>
	.container{
		position: absolute;
		top: 0;
		bottom: 0;
		left: 0;
		right: 0;
	}
	.invite_swiper{
		height: 100%;
	}
	.swiper-item{
		width: 100%;
		height: 100%;
		text-align: center;
	}
</style>
