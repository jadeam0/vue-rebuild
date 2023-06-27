<template>
    <div class="footer">
        <span class="footer-copy">© 2023 Company, Inc</span>

        <p class="footer-text">
            <router-like class="menu" to="/">Home</router-like>
            <router-like class="menu" to="/">About</router-like>
            <router-like class="menu" to="/">Products</router-like>
            <router-like class="menu" to="/">Admin</router-like>
        </p>
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
.footer {
    bottom: 0;
    left: 0;
    height: 90px;
    width: 100%;
    background-color: #aebcca;
}

.footer-text {
    font-size: 18px;
    padding-left: 30px;
    word-spacing: 100px;
}

.footer-copy {
    padding-top: 10px;
}

.menu {
    padding: 20px;
}

.menu:hover {
    background-color: rgb(200, 248, 248);
    font-size: 19px;
    color: black;
}

</style>