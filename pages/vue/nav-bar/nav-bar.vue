<template>
	<view>
		<uni-nav-bar :fixed="true" color="#ffffff" background-color="#007AFF" :status-bar="true" left-icon="arrowleft" left-text="返回" title="uni-nav-bar 标题"
		 @clickLeft="back" />
		<text class="example-info">本导航栏为自定义组件，并非原生导航栏。除非原生导航栏无法满足需求，否则不推荐使用自定义导航栏组件。具体参考https://ask.dcloud.net.cn/article/34921</text>
		<uni-section title="基本用法" type="line"></uni-section>
		<view class="example-body">
			<uni-nav-bar left-icon="arrowleft" title="标题" @clickLeft="back" />
		</view>

		<uni-section title="左右显示文字" type="line"></uni-section>
		<view class="example-body">
			<uni-nav-bar left-icon="arrowleft" right-text="菜单" left-text="返回" title="标题" @clickLeft="back" />
		</view>
		<uni-section title="插入slot" type="line"></uni-section>
		<view class="example-body">
			<uni-nav-bar :fixed="false" color="#333333" background-color="#FFFFFF" right-icon="scan" @clickLeft="showCity"
			 @clickRight="scan">
				<block slot="left">
					<view class="city">
						<view><text class="uni-nav-bar-text">{{ city }}</text></view>
						<uni-icons type="arrowdown" color="#333333" size="22" />
					</view>
				</block>
				<view class="input-view">
					<uni-icons class="input-uni-icon" type="search" size="22" color="#666666" />
					<input confirm-type="search" class="nav-bar-input" type="text" placeholder="输入搜索关键词" @confirm="confirm">
				</view>
			</uni-nav-bar>
		</view>
	</view>
</template>

<script>
	export default {
		components: {},
		data() {
			return {
				city: '北京'
			}
		},
		methods: {
			back() {
				uni.navigateBack({
					delta: 1
				})
			},
			showMenu() {
				uni.showToast({
					title: '菜单'
				})
			},
			clickLeft() {

				uni.showToast({
					title: '左侧按钮'
				})
			},
			search() {
				uni.showToast({
					title: '搜索'
				})
			},
			showCity() {

				uni.showToast({
					title: '选择城市'
				})
			},
			scan() {
				uni.showToast({
					title: '扫码'
				})
			},
			confirm() {
				uni.showToast({
					title: '搜索'
				})
			}
		},
		onPullDownRefresh() {
			console.log('onPullDownRefresh')
			setTimeout(function() {
				uni.stopPullDownRefresh()
				console.log('stopPullDownRefresh')
			}, 1000)
		}
	}
</script>

<style lang="scss" scoped>
	@import '@/common/uni-nvue.scss';
	$nav-height: 30px;
	
	page {
		height: 120%;
	}
	
	.uni-nav-bar-text {
		font-size: $uni-font-size-base;
	}

	.city {
		/* #ifndef APP-PLUS-NVUE */
		display: flex;
		/* #endif */
		flex-direction: row;
		align-items: center;
		justify-content: flex-start;
		// width: 160rpx;
		margin-left: 4px;
	}

	.input-view {
		/* #ifndef APP-PLUS-NVUE */
		display: flex;
		/* #endif */
		flex-direction: row;
		// width: 500rpx;
		flex: 1;
		background-color: $uni-bg-color-grey;
		height: $nav-height;
		border-radius: 15px;
		padding: 0 15px;
		flex-wrap: nowrap;
		margin: 7px 0;
		line-height: $nav-height;
	}

	.input-uni-icon {
		line-height: $nav-height;
	}

	.nav-bar-input {
		height: $nav-height;
		line-height: $nav-height;
		/* #ifdef APP-PLUS-NVUE */
		width: 370rpx;
		/* #endif */
		padding: 0 5px;
		font-size: $uni-font-size-base;
		background-color: $uni-bg-color-grey;
	}

	.example-body {
		/* #ifndef APP-NVUE */
		display: block;
		/* #endif */
		padding: 0;
	}
</style>
