<template>
<div>
            <section class="about">
              <div class="p-5 mb-4  rounded-3">
                <div class="container-fluid py-5">
                  <h1 class="display-5 fw-bold text-center">About Us</h1>
                  <p class="p-5 fs-5 text-center">At Anime Galore, we are passionate about all things anime. As dedicated fans ourselves, we understand the deep connection and joy that anime brings to people's lives. That's why we have made it our mission to provide a haven for fellow enthusiasts, offering a wide range of high-quality anime merchandise that captures the essence of your favorite shows and characters.</p>
                  <p class="px-5 fs-5 text-center">Anime Galore is more than just a shop – it's a community. We aim to foster a welcoming and inclusive space where fans can come together, celebrate their shared passions, and discover new favorites. Our knowledgeable and friendly team is always here to assist you, whether you're seeking recommendations, have questions about our products, or simply want to connect with fellow anime enthusiasts.</p>
                  <!-- <button class="btn btn-primary btn-lg" type="button">Example button</button> -->
                </div>
              </div>
              <div class="row align-items-md-stretch">
                <div class="col-md-6">
                  <div class="h-100 p-5 rounded-3 text-center mx-3" style="background: #FF4081; color: black;">
                    <h2>The Establishment</h2>
                    <p class="text-black">Anime Galore came to life from a passionate vision to celebrate the world of anime. Founded with love and dedication, we offer a curated selection of merchandise that captures the essence of beloved shows and characters. Join us on this incredible journey as we bring the magic of anime to fans worldwide.</p>
                    <!-- <button class="btn btn-outline-light" type="button">Example button</button> -->
                  </div>
                </div>
                <div class="col-md-6">
                  <div class="h-100 py-4 px-5 mx-3 bg-body-tertiary border rounded-3">
                    <img src="https://i.postimg.cc/1tJF84B4/346593060-1627565647720730-5260723005474733496-n.jpg" alt="shop-in" height="400" width="600" class="about-img">
                  </div>
                </div>
              </div>
              
              <div class="row align-items-md-stretch my-5">
                <div class="col-md-6">
                  <div class="h-100 py-4 px-5 mx-3 bg-body-tertiary border rounded-3">
                    <img src="https://i.postimg.cc/g2fZffSt/meeee.jpg" alt="owner" height="460" width="600" class="about-img">
                  </div>
                  
                </div>
                <div class="col-md-6">
                  <div class="h-100 p-5 rounded-3 text-center mx-3" style="background: #FF4081; color: black;">
                    <h2>The Founder</h2>
                    <p class="text-black">Meet the visionary behind Anime Galore, our company owner. With an unyielding passion for anime, they embarked on a mission to create a haven for fellow enthusiasts. Their deep understanding of the fandom and commitment to quality drive the curated collection we offer. Join us as we celebrate their love for anime and share in their journey of bringing the magic to life.</p>
                    <!-- <button class="btn btn-outline-light" type="button">Example button</button> -->
                  </div>
                </div>
              </div>
            </section>
            <section class="contact">
              <form action="https://formspree.io/f/xpzekzqg" method="POST" class="con mx-auto p-3 d-flex flex-column w-50 p-2 rounded-5" style="padding-top: 100px;">
                <label for="contact" class="text-center fs-1 m-5">Contact Us!</label>
                <div class="row m-2">
                  <div class="col-6">
                    <input type="text" class="form-control" placeholder="First name" aria-label="First name">
                  </div>
                  <div class="col-6">
                    <input type="text" class="form-control" placeholder="Last name" aria-label="Last name">
                  </div>
                </div>
                <div class="mb-3 m-3">
                  <!-- <label for="formGroupExampleInput" class="form-label">Example label</label> -->
                  <input type="text" class="form-control" id="formGroupExampleInput" placeholder="Email@">
                </div>
                <div class="form-floating m-3">
                  <textarea class="form-control" placeholder="Leave a comment here" id="floatingTextarea2" style="height: 100px; resize: none;"></textarea>
                  <label for="floatingTextarea2">Comments</label>
                </div>
                <button class="p-1 m-3" type="button">Submit!</button>
              </form>
            </section>
        </div>
</template>
