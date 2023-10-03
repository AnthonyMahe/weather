<template>
	<div>
		<h1>{{ title }}</h1>
		<Component01 />
	</div>
</template>

<script>
import Component01 from "../components/Component01.vue";

export default {
	name: "HomeView",
	data() {
		return {
			title: "HomeView",
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
	components: { Component01 },
};
</script>

<style scoped lang="scss">
/*
  style
*/
</style>
