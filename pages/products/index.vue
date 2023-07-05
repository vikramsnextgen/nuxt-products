<template>
    <div>
        <h1>products</h1>
        <div class="grid grid-cols-4 gap-5">
            <div v-for="p in products">
                <Card :product="p"/>
                <!-- <NuxtLink :to="`/products/${p.id}`">{{ p.title }}</NuxtLink> -->
            </div>
        </div>
    </div>
</template>

<script setup>
    definePageMeta({
        layout: 'products'
    })

    //fetch the products
    const {data:products} = await useFetch('https://fakestoreapi.com/products')


</script>

<style scoped>
    h2 {
        color: green;
    }
    p{
        color: blue;
    }
</Style>