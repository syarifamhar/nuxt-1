<template>
    <div>
        <h2>About</h2>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Provident, illum praesentium? Rerum, molestias debitis repellat cupiditate soluta eius similique, natus maiores nihil necessitatibus consectetur possimus, animi placeat sed voluptates eligendi!</p>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Provident, illum praesentium? Rerum, molestias debitis repellat cupiditate soluta eius similique, natus maiores nihil necessitatibus consectetur possimus, animi placeat sed voluptates eligendi!</p>
    </div>

    <div>
        {{ data }}
    </div>
</template>

<script setup>
const { data } = await useFetch('/api/default')

</script>

<style scoped>
 h2 {
    margin-bottom: 30px;
    font-size: 36px;
 }
 p {
    margin: 20px 0;
 }
</style>