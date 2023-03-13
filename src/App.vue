<template>
	<div class="my-layout">
		<HeaderComponent id="header" />
		<MainComponent id="main" />
		<FooterComponent id="footer" />
	</div>
</template>

<script>
import "./assets/style/variables.css";
import HeaderComponent from "./components/Header/HeaderComponent.vue";
import MainComponent from "./components/Main/MainComponent.vue";
import FooterComponent from "./components/Footer/FooterComponent.vue";

export default {
	name: "App",
	components: {
		HeaderComponent,
		MainComponent,
		FooterComponent,
	},
};
</script>

<style>
body {
	margin: 0;
}

.my-layout {
	display: grid;
	grid-template-rows: 88px 1fr 200px;
	grid-template-columns: 1fr;
	grid-template-areas:
		"header"
		"main"
		"footer";
}

#header {
	grid-area: header;
}

#main {
	grid-area: main;
}

#footer {
	grid-area: footer;
}

#app {
	font-family: "GT America Standard", sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
}
</style>
