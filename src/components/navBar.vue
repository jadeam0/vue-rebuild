<template>
    <nav class="topnav">
        <router-link class="active link" to="/">Home</router-link>
        <router-link class="link" to="/products">Products</router-link>
        <router-link class="link" to="/about">About</router-link>
        <router-link class="link" to="/admin">Admin</router-link>
    </nav>
</template>

<script>
export default {
    
}
</script>

<style scoped>
.topnav {
    background-color: #1976D2;
    overflow: hidden;
}

.link {
    text-align: center;
    color: #333;
    padding: 10px;
    text-decoration: none;
    font-size: 18px;
}

.link:hover {
    background-color: #7dbbf9;
    color: #333;
    font-size: 20px;
}

</style>