<script setup>
import { products } from "../stores/product.js";
</script>

<template>
	<div class="container mx-auto px-4">
		<search />
		<div class="grid grid-cols-4 gap-4">
			<div v-for="(product, id) in products" :key="id">
				<UCard>
					<p class="text-red-500 text-2xl">{{ product.title }}</p>
				</UCard>
			</div>
		</div>
	</div>
</template>
