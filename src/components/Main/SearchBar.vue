<template>
	<div class="search-bar">
		<span>Search</span>
	</div>
</template>

<script>
export default {};
</script>

<style scoped>
.search-bar {
	width: 70%;
	max-width: 720px;
	padding: 16px;

	background-color: var(--white-color);
	border: 1px solid black;
	border-radius: 4px;
	box-shadow: 0 9px 14px 0 rgb(0 0 0 / 10%);
}
.search-bar > span {
	font-size: 20px;
	color: #999999;
}
</style>
