<template>
	<view>
		<scroll-view scroll-y class="left-aside">
			<view v-for="item in flist" :key="item.id" class="f-item b-b" :class="{active: item.id === currentId}" @click="tabtap(item)">
				{{item}}
			</view>
		</scroll-view>
		
	</view>
</template>

<script>
	export default{
		data(){
			return{
				flist:["白酒","啤酒","葡萄酒","洋酒"]
				
			}
		}
	}
</script>

<style lang="scss">
	
</style>
