<template>
	<div class="home-Bloc">
		<div class="header">
			<h1>Mété</h1>
			<v-icon size='x-small' color="yellow" icon="fa-solid fa-sun" class="soleil"></v-icon>
		</div>
		<Component01 />
		<ChooseTown />
		<v-text-field label="Rechercher une ville"></v-text-field>
		<v-btn icon="fa-solid fa-plus" class="bouton"></v-btn>
	</div>
</template>

<script>
import Component01 from "../components/Component01.vue";
import ChooseTown from "../components/ChooseTown.vue";

export default {
	name: "HomeView",
	data() {
		return {
			title: "Météo" ,
		};
	},
	props: {},
	mounted() {
		// Mounted
	},
	methods: {
		// Methods
	},
	watch: {
		// Watchers
	},
	computed: {
		// Computed
	},
	components: { Component01, ChooseTown },
};
</script>

<style scoped lang="scss">
  .header {
	display: flex;
	justify-content: center;
	font-size: 2.5em;
	width: 100%;
	color: #f4d409;
	padding: 8px;
	border: 2px solid #f4d409;
	box-sizing: border-box;
	box-shadow: 0 0 8px #f4d409;
	max-width: 50%;
	margin: auto;
	max-width: 400px;
  }

  .soleil {
	transform: scale(95%);
  }

  .bouton {
	border: 2px solid white;
  }


</style>
