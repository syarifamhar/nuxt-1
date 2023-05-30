<template>
    <div class="mt-7 max-w-sm mx-auto text-center card">
        <h1 class="mt-7 text-7xl font-bold">{{ error.statusCode }}</h1>
        <p class="mt-7 text-5xl">Ooops...</p>
        <p class="mt-7">{{ error.message }}</p>
        <button class="btn" @click="handleClearError">To The Homepage</button>
    </div>
</template>

<script setup>
    defineProps(['error'])

    const handleClearError = () => clearError({ redirect:'/' })
</script>

<style scoped>

</style>