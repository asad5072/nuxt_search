<script setup>
const searchValue = ref("");

async function handleSearch() {
	navigateTo("/search/?search=" + searchValue.value);
}
</script>

<template>
	<div class="flex py-12">
		<input
			v-model="searchValue"
			type="search"
			name="search"
			placeholder="Search"
			class="border-2"
		/>
		<UButton @click="handleSearch" size="md" variant="solid" label="Search" />
	</div>
</template>
