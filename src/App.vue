<template>
	<div>
		<Header />
		<home />
		<Footer />
	</div>
</template>

<script>
import Header from './components/Header.vue';
import Home from './views/Home.vue';
import Footer from './components/Footer.vue';

export default {
	name: 'App',
	components: { Home, Header, Footer },
};
</script>

<style lang="scss" scoped></style>
