<script setup>
import { products } from "../stores/product.js";
const route = useRoute();
const { search } = route.query;

// const data = computed(() =>
// 	search ? products.filter((item) => item.title.includes(search)) : []
// );
const data = products.filter((item, index) =>
	item.title.toLowerCase().includes(search.toLowerCase())
);
</script>

<template>
	<div>
		<p>Search Results for: {{ search }}</p>
		<ul v-if="data.length">
			<li v-for="(item, index) in data" :key="index">
				{{ item.title }}
			</li>
		</ul>
		<p v-else>No results found.</p>
	</div>
</template>
