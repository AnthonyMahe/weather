<template>
	<div class="home-Bloc">
		<div class="header">
			<h1>Mété</h1>
			<v-icon size='x-small' color="yellow" icon="fa-solid fa-sun" class="soleil"></v-icon>
		</div>
		<!-- v-if ouvert permet de conditionner le composant ChooseTown -->
	<div class="infos">
		<ChooseTown v-if="ouvert" @close="fermerChooseTown"/>
		<v-btn icon="fa-solid fa-plus" class="bouton" @click="auClick" v-if="ouvert===false"></v-btn>
	</div>
	</div>
</template>

<script>
import ChooseTown from "../components/ChooseTown.vue";

export default {
	name: "HomeView",
	data() {
		return {
			title: "Météo" ,
			ouvert: false,
		};
	},
	props: {},
	mounted() {
		// Mounted
	},
	methods: {
		// Methods
		auClick() {
			this.ouvert= true
		},
		fermerChooseTown() {
			this.ouvert= false
		}
	},
	watch: {
		// Watchers
	},
	computed: {
		// Computed
	},
	components: { ChooseTown },
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
  
  .infos {
	display: flex;
	justify-content: center;
  }


</style>
