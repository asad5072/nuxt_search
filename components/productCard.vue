<script setup>
const products = [
	{
		title: "Wireless Bluetooth Headphones",
		description:
			"Noise-cancelling over-ear headphones with premium sound quality.",
		price: 89.99,
		rating: 4.7,
		image: "https://example.com/images/headphones.jpg",
	},
	{
		title: "4K Ultra HD Smart TV",
		description:
			"55-inch Smart TV with ultra HD resolution and streaming capabilities.",
		price: 599.99,
		rating: 4.5,
		image: "https://example.com/images/4ktv.jpg",
	},
	{
		title: "Stainless Steel Blender",
		description:
			"Powerful 1200W blender with multiple speed settings and a 64oz container.",
		price: 49.99,
		rating: 4.3,
		image: "https://example.com/images/blender.jpg",
	},
	{
		title: "Gaming Laptop",
		description:
			"High-performance laptop with Intel i7 processor, 16GB RAM, and NVIDIA GTX 3060.",
		price: 1099.99,
		rating: 4.8,
		image: "https://example.com/images/gaming-laptop.jpg",
	},
	{
		title: "Smartwatch with Fitness Tracker",
		description:
			"Waterproof smartwatch with heart rate monitor and GPS tracking.",
		price: 149.99,
		rating: 4.6,
		image: "https://example.com/images/smartwatch.jpg",
	},
	{
		title: "Portable Power Bank",
		description: "10,000mAh power bank with fast charging and dual USB ports.",
		price: 29.99,
		rating: 4.4,
		image: "https://example.com/images/powerbank.jpg",
	},
	{
		title: "Ergonomic Office Chair",
		description:
			"Adjustable office chair with lumbar support and breathable mesh back.",
		price: 179.99,
		rating: 4.2,
		image: "https://example.com/images/office-chair.jpg",
	},
	{
		title: "Electric Standing Desk",
		description:
			"Height-adjustable standing desk with memory presets and solid wood top.",
		price: 399.99,
		rating: 4.7,
		image: "https://example.com/images/standing-desk.jpg",
	},
	{
		title: "Air Fryer",
		description: "4-quart air fryer with digital display and non-stick basket.",
		price: 89.99,
		rating: 4.5,
		image: "https://example.com/images/airfryer.jpg",
	},
	{
		title: "Cordless Vacuum Cleaner",
		description:
			"Lightweight and powerful cordless vacuum with long battery life.",
		price: 199.99,
		rating: 4.6,
		image: "https://example.com/images/vacuum-cleaner.jpg",
	},
];
</script>

<template>
	<div class="container mx-auto px-4 py-12">
		<div class="grid grid-cols-4 gap-4">
			<div v-for="(product, id) in products" :key="id">
				<UCard>
					<p class="text-red-500 text-2xl">{{ product.title }}</p>
				</UCard>
			</div>
		</div>
	</div>
</template>
