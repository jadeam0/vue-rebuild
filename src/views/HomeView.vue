<template>
  <div>
            <section class="home-landing">
                <div class="home-text position-relative overflow-hidden p-3 p-md-5 m-md-3 text-center text-black">
                    <div class="col-md-5 p-lg-5 mx-auto my-5 text-black">
                        <h1 class="display-4 fw-semibold">Anime Galore</h1>
                        <h4 class="fs-4">Where Dreams Happen</h4>
                        <p  class="text-black fw-bold" >Come in and take a look; you might find a whole new world!</p>
                    </div>

                    <button type="button" class="shop-btn" href="./html/product.html">Shop Now!</button>
                </div>
            </section>
            <section>
                <div class="row d-flex align-content-center cate">
                    <div class="col-lg-4 d-flex flex-column align-items-center crd">
                      <img class="bd-placeholder-img rounded-circle" width="140" height="140" src="https://i.postimg.cc/ZRv8PK9j/figurines.jpg" role="img" aria-label="Placeholder" preserveAspectRatio="xMidYMid slice" focusable="false"><title>Placeholder</title><rect width="100%" height="100%" fill="var(--bs-secondary-color)"></rect>
                      <h2 class="fw-normal">figurines</h2>
                      <p>Unleash Anime Magic with Exquisite Figurines.</p>
                      <p><button type="button" href="./html/product.html">Take A Look!</button></p>
                    </div><!-- /.col-lg-4 -->
                    <div class="col-lg-4 d-flex flex-column align-items-center">
                      <img class="bd-placeholder-img rounded-circle" width="140" height="140" src="https://i.postimg.cc/c12DzCfR/plushies.jpg" role="img" aria-label="Placeholder" preserveAspectRatio="xMidYMid slice" focusable="false"><title>Placeholder</title><rect width="100%" height="100%" fill="var(--bs-secondary-color)"></rect>
                      <h2 class="fw-normal">Plushies</h2>
                      <p>Whimsical anime plushies for endless cuddles.</p>
                      <p><button type="button" href="./html/product.html">Take a Look!</button></p>
                    </div><!-- /.col-lg-4 -->
                    <div class="col-lg-4 d-flex flex-column align-items-center">
                      <img class="bd-placeholder-img rounded-circle" width="140" height="140" src="https://i.postimg.cc/sxrbt2hD/habitats.jpg" role="img" aria-label="Placeholder" preserveAspectRatio="xMidYMid slice" focusable="false"><title>Placeholder</title><rect width="100%" height="100%" fill="var(--bs-secondary-color)"></rect>
                      <h2 class="fw-normal">Habitats</h2>
                      <p>Anime-inspired habitats for imaginative adventures.</p>
                      <p><button type="button" href="./html/product.html">Take a Look!</button></p>
                    </div><!-- /.col-lg-4 -->
                  </div>
            </section>
        </div>
</template>

<script>

</script>

<style scoped>
::-webkit-scrollbar{
    display: none;
  }



.home-landing {
    height: 714px;
    background-image: url(https://i.postimg.cc/hjgbFgND/347375153-128320633597613-4368138262879456694-n.jpg);
    background-size: cover;
    background-position: top;
    position: relative;
    display: grid;
    grid-template-columns: repeat(1,1fr);
    align-items: center;
}

.home-text {
    color: black;
}

.home-text h1 {
    /* margin: 20px 0px 12px; */
    letter-spacing: 1.5px;
    font-weight: bolder;
    text-shadow: 0px 0px 5px #000, 0px 0px 18px #FF4081;
}

.home-text h4 {
    text-shadow: 0px 0px 5px #000, 0px 0px 18px #FF4081;
    font-size: 20px;
    letter-spacing: 2px;
    /* margin: 15px 0px 15px; */
}

.home-text p {
    color: black;
    font-size: large;
    text-shadow: 0px 0px 5px #000, 0px 0px 18px #FF4081;
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
