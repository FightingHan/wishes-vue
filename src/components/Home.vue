<template>
	<div class="nav">
		<div v-for="item in navList" :key="item.iconUrl" class="nav-item">
			<img :src="item.iconUrl" />
			<p>{{item.iconText}}</p>
		</div>
	</div>
</template>
<script>
	export default {
		data() {
			return {
				navList: [
					{
						iconText: "许愿池",
						iconUrl: require("../assets/images/location.png"),
					},
					{
						iconText: "写信！",
						iconUrl: require("../assets/images/edit.png"),
					},
					{
						iconText: "我的",
						iconUrl: require("../assets/images/girl.png"),
					},
				],
			};
		},
	};
</script>
<style lang="less" scoped>
.nav {
	position: fixed;
	bottom: 5px;
    display: flex;
	width: 100%;
	flex-direction: inherit;
	text-align: center;
	.nav-item {
		flex: 1;
		img {
			width: 30px;
			height: 30px;
		}
		span {
			font-size: 12px;
		}
	}
}
</style>