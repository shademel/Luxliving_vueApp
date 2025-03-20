<template>
  <nav></nav>
  <section class="bg-banner text-center">
    <div class="banner-img">
      <img src="../assets/Aboutus.jpg" alt="">
    </div>
    <div class="banner-blur"></div>
    <div class="container">
      <div class="row">
        <div class="col-lg-6 col-md-8">
          <h1 class="fw-bold text-white">About us</h1>
        </div>
      </div>
    </div>
    <header class="py-5 bg-color-primary text-white">
      <div class="container px-0 mt-5 py-5 my-5">
        <div class="row justify-content-center">
          <div class="col-lg-8 col-xxl-8 preload-rs">
            <div class="text-center my-5">
              <h1 class="fw-bolder mb-3">Our mission is to make highquality home and office furnitures easily accesible for everyone.</h1>
              <p class="lead fw-normal text-white-50 mb-4">Lux living was built on the idea of high quality, functional and beautiful products should be available and affordable to everyone. Use our platform to search and purchase high quality products.</p>
              <LinkButton btn-theme="secondary-btn" btn-label="Start shopping Now" btn-url="" btn-icon="arrow-right" outlined="false" class="btn-lg mt-3" />
            </div>
          </div>          
        </div>
      </div>
    </header>
  </section>
  
  <section class="py-5 my-5" id="features">
    <div class="container px-4 pb-5 mb-5 mt-3">
      <div class="row justify-content-between align-items-center">
        <div class="col-lg-5 ps-0 ms-0 preload-rs s-anim">
          <div class="header">
            <h1 class="h1 fw-bolder">Why Us</h1>
            <p class="fw-normal lead mb-3">We guarantee satisfaction service, ensuring an exceptional shopping experience for every customer.</p>
          </div>
          <div class="row gx-5">
            <div class="col-6 col-md-6 mb-5 mb-lg-0 my-4">
              <span class="icon h1 fw-bolder mb-3 d-block"><i class="bi bi-truck"></i></span>
              <h2 class="h5 fw-bolder">Fast & Free Shipping</h2>
              <p>Your furnitures will be delivered to you quickly</p>
            </div>
            <div class="col-6 col-md-6 mb-5 mb-lg-0 my-4">
              <span class="icon h1 fw-bolder mb-3 d-block"><i class="bi bi-bag-check"></i></span>
              <h2 class="h5 fw-bolder">Easy to Shop</h2>
              <p>Purchase furniture with our friendly platform</p>
            </div>
            <div class="col-6 col-md-6 mb-5 mb-lg-0 my-4">
              <span class="icon h1 fw-bolder mb-3 d-block"><i class="bi bi-headset"></i></span>
              <h2 class="h5 fw-bolder">24/7 Customer Support</h2>
              <p>Receive 24/7 customer support</p>
            </div>
          </div>
        </div>
        <div class="col-lg-6 mt-5 mt-lg-0 preload-rs s-anim">
          <div class="img-wrap">
            <div class="img-grid grid-lg ">
              <img src="" alt="" >
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <br>
  <section class="mt-5 py-5 bg-light" id="team">
    <div class="container px-5 my-5 py-5 row">
      <div class="text-center">
        <h2 class="fw-bolder">Our Team</h2>
        <p class="lead fw-normal text-muted mb-5">Meet our dedicated individual. From our leaders to designers and customer support team. Our team is committed to providing you with the best shopping experience possible.</p>
      </div>
      <div class="row gx-5 row-cols-1 row-cols-sm-2 row-cols-xl-4 justify-content-center">
        <div class="col mb-5 mb-xl-0 preload-rs s-anim row">
          <div class="text-center column">
            <img src="../assets/person-1.jpg" alt="Avatar" class="avatar">
            <h5 class="fw-bolder">Abby</h5>
            <span class="d-block position mb-4 text-black-50">Co-Founder, Lux Living</span>
            <p class="mb-0 fw-semibold text-u"><a href="#" class="more dark">View Profile <span class="bi bi-arrow-right ms-2"></span></a></p>
          </div>
        </div>
        <div class="col mb-5 mb-xl-0 preload-rs s-anim">
          <div class="text-center column">
            <img src="../assets/person-3.jpg" alt="Avatar" class="avatar">
            <h5 class="fw-bolder">Ben</h5>
            <span class="d-block position mb-4 text-black-50">Co-Founder, Lux Living</span>
            <p class="mb-0 fw-semibold text-u"><a href="#" class="more dark">View Profile <span class="bi bi-arrow-right ms-2"></span></a></p>
          </div>
        </div>
        <div class="col mb-5 mx-xl-0 preload-rs s-anim">
          <div class="text-center column">
            <img src="../assets/person-2.jpg" alt="Avatar" class="avatar">
            <h5 class="fw-bolder">Jackie</h5>
            <span class="d-block position mb-4 text-black-50">Customer support, Lux Living</span>
            <p class="mb-0 fw-semibold text-u"><a href="#" class="more dark">View Profile <span class="bi bi-arrow-right ms-2"></span></a></p>
          </div>
        </div>
        <div class="col mb-5 mb-xl-0 preload-rs s-anim">
          <div class="text-center column">
            <img src="../assets/person-4.jpg" alt="Avatar" class="avatar">
            <h5 class="fw-bolder">Max</h5>
            <span class="d-block position mb-4 text-black-50">Customer support, Lux Living</span>
            <p class="mb-0 fw-semibold text-u"><a href="#" class="more dark">View Profile <span class="bi bi-arrow-right ms-2"></span></a></p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>

</script>

<style>
.container {
  background-color: #0d0b0b;
}

.avatar {
  border-radius: 50%;
  vertical-align: middle;
  height: 120px;
  width: 120px;
}

.bg-banner {
    overflow: hidden;
    position: relative;
}

.bg-banner .banner-img {
    width: 100%;
    height: 100%;
    z-index: -1;
    top: 0;
    left: 0;
    position: absolute;
}

.bg-banner .banner-img img {
    height: 100%;
    width: 100%;
    max-width: 100%;
    object-position: center;
    object-fit: cover;
}

.bg-banner .banner-blur {
    width: 100%;
    height: 100%;
    z-index: -1;
    opacity: 0.5;
    position: absolute;
    top: 0;
    left: 0;
}
</style>