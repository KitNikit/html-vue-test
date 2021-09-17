<template>
	<p class="file">
		<img
			src="https://cdn2.iconfinder.com/data/icons/kids/128x128/actions/editcopy.png"
		/>
		{{ name }}
	</p>
</template>

<script>
export default {
	name: 'FileView',
	props: {
		name: String,
	},
};
</script>

<style scoped lang="scss">
.file {
	color: green;
	width: 200px;
	height: 40px;
	background: #3e4363;
	border: 1px solid #ce7077;
	border-radius: 10px;
	box-shadow: 5px 5px 10px #3e4363;
	display: flex;
	align-items: center;
	justify-content: space-around;
	font-weight: bold;
	cursor: pointer;
	transition: transform 0.3s ease-out;
	img {
		height: 30px;
	}
	&:hover {
		transform: scale(1.2);
	}
	&:active {
		color: white;
	}
}
</style>
