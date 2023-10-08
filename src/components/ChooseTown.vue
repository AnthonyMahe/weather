<template>
	<div>
		<h1>{{ title }}</h1>
		<v-btn icon="fa-solid fa-xmark" class="bouton" @click="auClick"></v-btn>
		<v-text-field label="Rechercher une ville"></v-text-field>
	</div>
</template>

<script>
export default {
	name: "ChooseTown",
	data() {
		return {
			title: "",
		};
	},
	props: {},
	mounted() {
		// Mounted
	},
	methods: {
		// Methods
		auClick() {
			this.$emit("close")
		}
	},
	watch: {
		// Watchers
	},
	computed: {
		// Computed
	},
};
</script>

<style scoped lang="scss">
/*
  style
*/
</style>
