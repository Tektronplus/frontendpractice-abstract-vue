<template>
	<div class="container-item">
		<span class="title">{{ title }}</span>
		<span class="description">{{ description }}</span>
		<img
			class="img-item"
			:src="urlImg"
			:alt="altImg" />
		<a
			class="link"
			href="#">
			Learn More
			<i class="lni lni-arrow-right"></i>
		</a>
	</div>
</template>

<script>
export default {
	components: {},
	props: {
		title: String,
		description: String,
		urlImg: String,
		altImg: String,
	},
};
</script>

<style scoped>
.container-item {
	display: grid;
	grid-template-rows: auto auto auto;
	grid-template-columns: 90px 1fr;
	grid-template-areas:
		"img title"
		"img description"
		"img link";
	gap: 10px 20px;
}
.title {
	grid-area: title;
	font-weight: bold;
	font-size: 24px;
}

.description {
	grid-area: description;
	font-size: 24px;
}
.img-item {
	grid-area: img;

	width: 100%;
	max-width: 90px;
	height: auto;
}
.link {
	grid-area: link;

	color: #4c5fd5;
	font-size: 20px;
	text-decoration: none;
}

.link:hover {
	text-decoration: underline;
}
</style>
