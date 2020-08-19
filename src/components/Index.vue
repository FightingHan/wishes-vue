<template>
	<div id="body">
		<div id="map">
			<div class="header">
				<input type="text" placeholder="请输入地址" />
				<button>搜索</button>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		data() {
			return {};
		},
	};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
#body {
	padding: 10px;
}
.header {
	height: 40px;
	box-shadow: 0 3px 3px rgba(10, 16, 20, 0.24), 0 3px 3px rgba(10, 16, 20, 0.24);
	display: flex;
	input {
		border-style: none;
		flex: 1;
		padding-left: 10px;
	}
	button {
		width: 60px;
		background-color: #cc3399;
		border-style: none;
		color: #ffffff;
		font-size: 16px;
	}
}
</style>
