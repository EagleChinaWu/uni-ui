<template>
	<view class="page">
		<text class="example-info">可以同时选择日期和时间的选择器</text>
		<uni-section :title="'基本用法：' + datetime" type="line"></uni-section>
		<view class="example-body">
			<uni-datetime-picker :value="datetime" @change="datetimeChange"></uni-datetime-picker>
		</view>
		<uni-section :title="'v-model用法：' + vModelDatetime" type="line"></uni-section>
		<view class="example-body">
			<uni-datetime-picker v-model="vModelDatetime" start="2010-6-10 08:30:30" end="2015-6-10 08:30:30"></uni-datetime-picker>
		</view>
		<uni-section :title="'无边框用法：' + vModelDatetime" type="line"></uni-section>
		<view class="example-body">
			<uni-datetime-picker v-model="vModelDatetime" :border="false" start="2010-6-10 09:30:30" end="2015-6-10 08:30:30"></uni-datetime-picker>
		</view>
		<uni-section :title="'不选秒（没有秒）用法：' + noSecond" type="line"></uni-section>
		<view class="example-body">
			<uni-datetime-picker v-model="noSecond" :hide-second="true" start="2010-6-10 08:30:30" end="2015-6-10 08:30:30"></uni-datetime-picker>
		</view>
		<uni-section :title="'disabled用法：' + disDatetime" type="line"></uni-section>
		<view class="example-body">
			<uni-datetime-picker disabled v-model="disDatetime"></uni-datetime-picker>
		</view>
		<uni-section :title="'时间戳用法：' + timestamp" type="line"></uni-section>
		<view class="example-body">
			<uni-datetime-picker :value="timestamp" return-type="timestamp" start="1276129830000" end="1623285030000" @change="timestampChange"></uni-datetime-picker>
		</view>
		<uni-section :title="'选择日期用法：' + date" type="line"></uni-section>
		<view class="example-body">
			<uni-datetime-picker type="date" :value="date" start="2020-2-31" end="2025-2-30" @change="dateChange"></uni-datetime-picker>
		</view>
		<uni-section :title="'选择时间用法：' + time" type="line"></uni-section>
		<view class="example-body">
			<uni-datetime-picker type="time" :value="time" start="16:30:30" end="20:30:30" @change="timeChange"></uni-datetime-picker>
		</view>
		<uni-section :title="'时分（没有秒）用法：' + timeNoSecond" type="line"></uni-section>
		<view class="example-body">
			<uni-datetime-picker type="time" v-model="timeNoSecond" hide-second="true"  start="16:30:30" end="20:30:30" return-type="timestamp"></uni-datetime-picker>
		</view>
		<uni-section :title="'（2021-06-01 06:30:20） ~ （2021-06-01 06:30:30） 起始日期用法：' + timeArea" type="line"></uni-section>
		<view class="example-body">
			<uni-datetime-picker :value="timeArea" start="2021-06-01 06:30:20" end="2021-06-01 06:30:30" @change="timeAreaChange"></uni-datetime-picker>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				datetime: '2021/02/013 09:30:00',
				vModelDatetime: '',
				noSecond: '2014-06-10 04:28:30',
				disDatetime: '2021-02-013 00:00:00',
				date: '2000-6-15',
				time: '17:30:30',
				timeNoSecond: '17:30',
				timestamp: 1610364547000,
				timeArea: ''
			}
		},
		mounted() {
			setTimeout(() => {
				this.vModelDatetime ='2021-03-01'
			}, 3000)
		},
		methods: {
			datetimeChange(e) {
				this.datetime = e
			},
			dateChange(e) {
				this.date = e
			},
			timeChange(e) {
				this.time = e
			},
			timestampChange(e) {
				this.timestamp = e
			},
			timeAreaChange(e) {
				this.timeArea = e
			}
		}
	}
</script>

<style lang="scss">
	@import '@/common/uni-nvue.scss';
</style>
