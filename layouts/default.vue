<template>
    <div>
        <header class="shadow-lg bg-slate-500 border-slate-600">
            <nav class="container flex mx-auto p-4 justify-between">
                <NuxtLink to="/" class="font-bold text-lg">First Nuxt</NuxtLink>
                <ul class="flex gap-4">
                    <li><NuxtLink to="/">Home</NuxtLink></li>
                    <li><NuxtLink to="/about">About</NuxtLink></li>
                    <li><NuxtLink to="/product" class="btn">Product</NuxtLink></li>
                </ul>
            </nav>
        </header>

        <!-- Output of contents -->
        <div class="container mx-auto p-4">
            <slot /> 
        </div>
    </div>
</template>

<style scoped>
.router-link-exact-active {
    color: #12b488;
}
</style>