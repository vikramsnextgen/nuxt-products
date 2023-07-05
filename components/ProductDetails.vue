<template>
    <div class="card">
        <div class="grid grid-cols-2gap-10">
            <div class="p-7">
                <img :src="product.image" alt="" srcset="" class="mx-auto my-7">
            </div>
            <div class="p-7">
                <h2 class="text-4x1 my-7">{{ product.title }}</h2>
                <p class="text-xl my-7">price - ${{ product.price }}</p>
                <h3 class="font-bold border-b-2 mb-4 pb-2">product description</h3>
                <p class="mb-7">{{ product.description }}</p>
            </div>
        </div>
    </div>
</template>

<script setup>
    const {product} = defineProps(['product'])
</script>

<style scoped>
    .thumb{
        max-height: 120px;
        max-width: 70%;
        margin:0 auto;
    }

    img {
        width: 400px;
    }
</style>