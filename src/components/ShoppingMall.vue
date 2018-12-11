<template>
	<div class="search-bar">
		<van-row gutter="5">
			<van-col span="3"><i class="iconfont icon-locationfill noraml-icon"></i></van-col>
			<van-col span="16">
				<input type="text" class="search-input"/>
			</van-col>
			<van-col span="5">搜索</van-col>
		</van-row>
	</div>
</template>

<script>
export default {
	data() {
		return {
			msg: "welcome to e-business"
		};
	}
};
</script>

<style scoped>
.search-bar{
    height: 2.2rem;
    background-color: #109ee8;
	line-height:2.2rem;
	font-size: 0.9rem;
	color: #fff;
}

.search-input{
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
</style>