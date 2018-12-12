<template>
	<div>
		<div class="search-bar">
			<van-row gutter="5">
				<van-col span="3"><i class="iconfont icon-locationfill noraml-icon"></i></van-col>
				<van-col span="16">
					<input type="text" class="search-input"/>
				</van-col>
				<van-col span="5">搜索</van-col>
			</van-row>
		</div>
		<div class="swiper-area">
			<van-swipe :autoplay="2000">
				<van-swipe-item v-for="(banner,index) in bannerPicArray" :key="index">
					<img :src="banner.imageUrl" v-lazy="banner.imageUrl" width="100%"/>
				</van-swipe-item>
			</van-swipe>
		</div>
	</div>
</template>

<script>

export default {
	data() {
		return {
			bannerPicArray:[
                {imageUrl:'https://img.yzcdn.cn/public_files/2017/09/05/3bd347e44233a868c99cf0fe560232be.jpg'},
                {imageUrl:'https://img.yzcdn.cn/public_files/2017/09/05/c0dab461920687911536621b345a0bc9.jpg'},
                {imageUrl:'https://img.yzcdn.cn/public_files/2017/09/05/4e3ea0898b1c2c416eec8c11c5360833.jpg'}
            ]
		};
	}
};
</script>

<style scoped>
.search-bar {
    height: 2.2rem;
    background-color: #109ee8;
	line-height:2.2rem;
	font-size: 0.9rem;
	color: #fff;
}

.search-input {
    width:100%;
	height: 1.4rem;
	border-radius: 1.4rem;
	background: #fff;
	border: 0;
	padding: 0 0.7rem;
	box-sizing: border-box;
	font-size: 0.9rem;
	color: #666;
}

.swiper-area{
    width:20rem;
    clear:both;
}
</style>