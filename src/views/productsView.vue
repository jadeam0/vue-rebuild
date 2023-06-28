<template>
    <button @click="sortPrice">Sort by Price</button>
    <input type="text" v-model="search" placeholder="Search...">
    <select v-model="area">
        <option value="All">All</option>
        <option value="Figurines">Figurines</option>
        <option value="Habitats">Habitats</option>
        <option value="Plushies">Plushies</option>
    </select>
    <div v-if="Products" class="flex-container">
        <ProductCard v-for="product of products" :key="product.id" :product="product"/>
    </div>
    <div v-else>Loading...</div>


    <div v-if="products" class="flex-container">
        <CardComp v-for="product of products" :key="product.id" :product="product"/>
    </div>

    <div v-else>Loading...</div>
</template>

<script>
import CardComp from '@/components/productCard.vue';
import ProductCard from '@/components/productCard.vue';

export default {

    data() {
        return {
            search:"",
            area: "All"
        }
    },

    methods: {
        sortPrice() {
            this.$store.commit("sortProductsByPrice")
        }
    },

    computed: {
        products() {
            return this.$store.state.products?.filter((product) => {
                let isMatch = true;
                if (!product.name.toLowerCase().includes(this.search.toLowerCase())) {
                    isMatch = false;
                }
                if (this.area !== "All" && this.area !== product.area) {
                    isMatch = false
                }
                return isMatch
            })
        }
    },

    mounted() {
        this.$store.dispatch("getProducts")
    },

    components: {
        CardComp,
        ProductCard
    }
}
</script>