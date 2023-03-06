<template>
	<div id="help-seeker-container">
		<span id="title-help-seeker">How can we help?</span>
		<SearchBar />
	</div>
</template>

<script>
import SearchBar from "./SearchBar.vue";
export default {
	components: {
		SearchBar,
	},
};
</script>

<style scoped>
#help-seeker-container {
	padding-top: 80px;
	padding-bottom: 80px;
	background-color: var(--purple-color);

	display: flex;
	flex-direction: column;
	align-items: center;
	justify-content: center;
	gap: 16px;
}

#title-help-seeker {
	font-size: 80px;
}
</style>
