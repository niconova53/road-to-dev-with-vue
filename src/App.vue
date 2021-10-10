<template>
	<div>
		<layout class="bg-light">
			<home slot="home" />
		</layout>
	</div>
</template>

<script>
import Home from '@/views/Home.vue';
import Layout from '@/components/Layout.vue';
export default {
	name: 'App',
	components: { Home, Layout },
};
</script>

<style lang="scss" scoped></style>
