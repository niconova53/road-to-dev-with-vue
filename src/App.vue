<template>
	<div>
		<home />
		<Header />
		<Footer />
	</div>
</template>

<script>
import Header from './components/Header.vue';
import Home from './views/Home.vue';
import Footer from './components/Footer.vue';

export default {
	components: { Home, Header, Footer },
	name: 'App',
};
</script>

<style lang="scss" scoped></style>
