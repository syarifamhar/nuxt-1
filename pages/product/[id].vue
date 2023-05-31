<template>
    <head>
        <Title>Learn Nuxt 3 | {{ product.title }}</Title>
        <meta name="description" :content="product.description">
    </head>

    <div>
        <ProductDetails :product="product" />
    </div>
</template>

<script setup>
    const { id } = useRoute().params
    const uri = 'https://fakestoreapi.com/products/' + id

    //fetch the product
    const { data: product } = await useFetch(uri) 

    if (!product.value) {
        throw createError ({ statusCode: 404, statusMessage: 'Product Not Found, make sure you find the right product!', fatal: true})
    }

    definePageMeta ({
    layout: 'product'
})
</script>

<style scoped>

</style>