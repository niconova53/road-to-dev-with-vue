<template>
	<div class="layout">
		<Header />
		<div>
			<slot name="home"></slot>
		</div>
		<Footer />
	</div>
</template>

<script>
import Header from './Header.vue';
import Footer from './Footer.vue';
export default {
	components: {
		Header,
		Footer,
	},
};
</script>

<style scoped>
.layout {
	height: 100%;
}
</style>
