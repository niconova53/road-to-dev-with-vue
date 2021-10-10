<template>
	<div class="card-group">
		<Card
			v-for="(pokemon, index) in pokemons"
			:key="index"
			:name="pokemon.name"
			:url="pokemon.url"
			class="col-4 card-enhance"
		/>
	</div>
</template>

<script>
import Card from './Card.vue';
import axios from 'axios';
export default {
	data() {
		return {
			pokemons: [],
			generation: 1,
		};
	},
	components: {
		Card,
	},
	created() {
		this.fetchData(3);
	},
	methods: {
		async fetchData(gen) {
			try {
				let pokemones = await axios.get(
					`https://pokeapi.co/api/v2/generation/${gen}`
				);
				let data = await pokemones.data.pokemon_species;

				this.pokemons = data;
			} catch (error) {
				console.log(error);
			}
		},
	},
};
</script>

<style scoped>
.card-container {
	display: flex;
	justify-content: center;
	align-items: center;
}
.card-enhance {
	min-width: unset;
}
</style>
