<template>
	<view class="content">
		<view class="list" @touchstart="$refs.add.closeAnimation()">
			<view class="listItem" v-for="(item,index) in 10">
				item{{index}}
			</view>
		</view>
		<wm-list-add ref="add" @clickAdd="clickAdd"/>
	</view>
</template>

<script>
	import wmListAdd from '@/components/wm-list-add/wm-list-add';
	export default {
		comments:{
			wmListAdd
		},
		data() {
			return {
			}
		},
		onLoad() {
		},
		methods: {
			clickAdd(){
				console.log('点击加号执行操作')
			}
		}
	}
</script>

<style>
	page{
		background-color: #f2f2f2;
	}
	.listItem{
		padding: 30rpx;
		background: #ffffff;
		border-radius: 10rpx;
		line-height: 80rpx;
		margin: 20rpx;
		margin-bottom: 0;
	}
</style>
