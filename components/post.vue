<template>
	<view class="post">
		<u-avatar class="post-avatar" :text="text"></u-avatar>
		<view class="post-body">
			<view class="post-body-head">
				<u--text type="primary" text="用户名1"></u--text>
				<u--text type="info" text="一分钟前"></u--text>
			</view>
			<view class="post-body-content">
				<u-tag text="恭喜" size="mini" type="error"></u-tag>
				<u--text text="这是ECNU-X论坛的第一条帖子"></u--text>
			</view>
			<view class="post-body-foot">
				<u--image :showLoading="true" :src="src" width="80px" height="80px"></u--image>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		name:"post",
		data() {
			return {
				src: 'https://cdn.uviewui.com/uview/album/1.jpg',
				text:'X'
			};
		}
	}
</script>

<style lang="scss">
.post{
	padding: 10px 0;
	display: flex;
	background-color: #efefef;
	&-avatar{
		width: 50px;
	}
	&-body{
		margin: 0 10px;
		display: flex;
		justify-content: space-between;
		flex-direction: column;
		&-head{
			display: flex;
		}
		&-content{
			display: flex;
		}
	}
}
</style>