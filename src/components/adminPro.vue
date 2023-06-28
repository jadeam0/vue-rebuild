<template>
    <tr>
        <td>{{ product.id }}</td>
        <td>{{ product.name }}</td>
        <td><img :src="product.image" :alt="product.name" ></td>
        <td>{{ product.price }}</td>
        <td>{{ product.quantity }}</td>
        <td>{{ product.category }}</td>
        <td>
            <a class="btn" @click="deleteProduct()">Delete</a>
            <a class="btn" @click="editProduct()">Edit</a>
        </td>
    </tr>
</template>

<script>
export default {
    props:["product"]
}
</script>

<style scoped>
img {
    width: 100px;
    height: 100px;
}
</style>