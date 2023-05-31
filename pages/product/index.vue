<template>
    <div>
        <div class="grid grid-cols-4 gap-5">
            <div v-for="p in products" :key="p">
                <ProductCard :product="p" />
            </div>
        </div>
    </div>
</template>

<script setup lang="ts">
definePageMeta ({
    layout: 'product'
})

//fetch all the products
const { data: products } = await useFetch ('https://fakestoreapi.com/products')

useHead ({
    title: 'Learn Nuxt 3 | Shop',
    meta: [
        {name: 'description', content: 'Learn Nuxt 3 Shop'}
    ]
})
</script>

<style scoped>

</style>