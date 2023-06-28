<template>
    <div class="main-content">
        <div class="row">
            <div class="col-md-12">
                <div class="table-wrapper">
                    <div class="table-title">
                        <div class="row">
                            <div class="col-sm-6 p-0 d-flex justify-content-lg-start justify-content-center">
                                <h2 class="ml-lg-2 m-3">Manage Products</h2>
                            </div>
                            <div class="col-sm-6 p-0 d-flex justify-content-lg-end justify-content-center my-2 mx-auto">
                                <!-- <button href="#addProductModal" onclick="addProduct()" class="p-0" data-toggle="modal" data-bs-target="#addProductModal">
                                    <i class="material-icons">&#xE147;</i> <span>Add New Product</span></button> -->
                                <button type="button" class="" data-bs-toggle="modal" data-bs-target="#addProductModal">
                                    Add New Product
                                </button>
                                <button href="#deleteProductModal" class="" data-toggle="modal">
                                    <i class="material-icons">&#xE15C;</i> <span>Delete</span></button>
                            </div>
                        </div>
                    </div>
            
                    <table class="table table-striped table-hover">
                        <thead>
                            <tr>
                                <th>ID</th>
                                <th>Name</th>
                                <th>Image</th>
                                <th>Price</th>
                                <th>Quantity</th>
                                <th>Category</th>
                                <th>Actions</th>
                            </tr>
                        </thead>

                        <tbody id="add-rmv-prod" v-if="products" class="flex-container">
                            <AdminProComp v-for="product of products" :key="product.id" :product="product"/>
                        </tbody>

                        <!-- <table class="productInfo">

                        </table> -->
                    </table>
                </div>
            </div>
        </div>
    </div>
    

<!-- Edit Modal HTML -->

<div id="addProductModal" class="modal fade">
    <div class="modal-dialog">
        <div class="modal-content">
            <form>
                <div class="modal-header">
                    <h4 class="modal-title">Add Product</h4>
                    <button type="button" class="close p-0" data-dismiss="modal" aria-hidden="true">&times;</button>
                </div>

                <div class="modal-body">
                    <div class="form-group">
                        <label>Name</label>
                        <input type="text" class="form-control" required id="name">
                    </div>
                    <div class="form-group">
                        <label>Image</label>
                        <input type="text" class="form-control" required id="preview">
                    </div>
                    <div class="form-group">
                        <label>Quantity</label>
                        <input  type="number" class="form-control" required id="quantity">
                    </div>
                    <div class="form-group">
                        <label>Category</label>
                        <input type="text" class="form-control" required id="category">
                    </div>
                </div>

                <div class="modal-footer">
                    <input type="button" class="btn btn-default" data-dismiss="modal" value="Cancel">
                    <input type="submit" class="btn btn-success productInfo" value="Add" onclick="addProduct() ">
                </div>
            </form>
        </div>
    </div>
</div>

</template>

<script>
import AdminProComp from '@/components/adminPro.vue'

export default {
    
    computed: {
        products() {
            return this.$store.state.products
        }
    },

    mounted() {
        this.$store.dispatch("getProducts")
    },

    components: {
        AdminProComp
    }
}
</script>

<style scoped>
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