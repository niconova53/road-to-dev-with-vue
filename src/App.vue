<template>
	<div>
		<hello-world msg="Hola VUE!" />
		<button class="btn btn-primary">Hola como va</button>
	</div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';

export default {
	name: 'App',
	components: { HelloWorld },
};
</script>

<style lang="scss" scoped></style>
