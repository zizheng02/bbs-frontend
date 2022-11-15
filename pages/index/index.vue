<template>
	<view class="content">
		<post></post>
	</view>
</template>

<script>
	import post from '../../components/post.vue'
	export default {
		components:{
			post
		},
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

<style>
	.content {
		margin: 10px 10px;
	}
</style>
