<template>
	<div class="card mx-4 mb-3">
		<img src="@/assets/perro.jpg" class="card-img-top" alt="perro" />
		<div class="card-body">
			<h5 class="card-title">{{ name }}</h5>
			<p class="card-text">
				<a href="#">{{ url }}</a>
			</p>
			<p class="card-text">
				<small class="text-muted">Last updated 3 mins ago</small>
			</p>
		</div>
	</div>
</template>

<script>
export default {
	name: 'Card',
	props: {
		name: { type: String, require: true, default: 'Loading' },
		url: { type: String, require: false },
	},
	data() {
		return {};
	},
};
</script>

<style></style>
