<template>
    <div class="card text-center">
        <img :src="product.image" alt="product thumb" class="thumb">
        <p class="text-gray font-bold m-4 truncate">{{ product.title }}</p>
        <NuxtLink :to="`/products/${product.id}`">
            <p class="btn my-4">View Details</p>
        </NuxtLink>

    </div>
</template>

<script setup>
    const {product} = defineProps(['product']);
</script>

<style scoped>
    .card{
        display: grid;
    }
</style>