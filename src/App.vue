<template>
	<FolderView name="$" :folders="folders" :files="files" />
</template>

<script>
import FolderView from './components/FolderView.vue';
import data from './data/list';

export default {
	name: 'App',
	components: {
		FolderView,
	},
	data: () => data,
};
</script>

<style lang="scss">
#app {
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	padding: 20px;
	background: url(https://vsthemes.org/uploads/posts/2020-08/1598709615_screenshot_1.jpg)
		center center / cover no-repeat;
}
</style>
