<template>
    <router-link :to="{name: 'product', params: {id: product.id}}">
        
        <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-3 m-2" id="figurines">
            <div class="col">
                <div div class="card shadow-sm">
                    <img class="bd-placeholder-img card-img-top" width="120px" height="350" :src="product.image" role="img" aria-label="Placeholder: Thumbnail" preserveAspectRatio="xMidYMid slice" focusable="false">
                    <div class="card-body">
                        <h5 class="card-title fs-5">{{ product.name }}</h5>
                        <p class="card-text fs-6">R {{product.price }}</p>

                        <div class="d-flex justify-content-between align-items-center">
                            <div class="btn-group">
                                <button id="addToCart" @click="addToCart( 'product.id' )" class="p-0">Add to Cart</button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </router-link>
</template>

<script>
export default {
    props: ["product"]
}
</script>

<style scoped>
.btn-group {
    text-decoration: none;
}

button {
    background-color: #eee;
    border: none;
    padding: 1rem;
    font-size: 1rem;
    width: 10em;
    border-radius: 1rem;
    color:  #FF4081;
    box-shadow: 0 0.4rem #dfd9d9;
    cursor: pointer;
    /* text-decoration: none; */
   }
   
   button :active {
    color: white;
    box-shadow: 0 0.2rem #dfd9d9;
    transform: translateY(0.2rem);
   }
   
   button:hover:not(:disabled) {
    background:  #FF4081;
    color: white;
    text-shadow: 0 0.1rem #bcb4b4;
   }
   
   button :disabled {
    cursor: auto;
    color: grey;
   }
</style>