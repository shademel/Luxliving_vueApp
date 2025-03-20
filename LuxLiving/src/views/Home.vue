<template>
    <nav active="home"></nav>
    <main class="main">
        <div class="mainbanner d-flex align-items-center">
            <div class="container">
                <div class="content">
                    <div class="preload">
                        <h1>Home furnitures</h1>
                        <p>Furniture brings you comfort</p>
                        <button btn-label="Explore More" btn-icon="arrow-right" btn-url="shop" class="btn-lg mt-3" btn-theme="secondary-btn">Explore More</button>
                    </div>
                </div>
                <br>
                <div class="search">
                    <label class="hide-ally-element" for="search">keyword search</label>
                    <input type="text" id="search" ref="search" placeholder="search here...">
                    <i class="fas fa-search"></i>
                </div>
                <br>
                <div class="banner-image">
                    <img class="main-banner-img" src="../assets/main-banner.jpg">
                </div>
            </div>
        </div>

        <div class="">
            <div class="container">
                <div class="row row-cols-1 row-cols-lg-4">
                    <div class="feature" align="center">
                        <img class="icon-img" src="">
                        <p class="fw-semibold">Free Delivery</p>
                        <span class="fw-semibold color-black">Free delivery for all products</span>
                    </div>
                    <div class="feature" align="center">
                        <img class="icon-img" src="">
                        <p class="fw-semibold">Free Return</p>
                        <span class="fw-semibold color-black">Free returns for all products</span>
                    </div>
                    <div class="feature" align="center">
                        <img class="icon-img" src="">
                        <p class="fw-semibold">Support 24/7</p>
                        <span class="fw-semibold color-black">Customer support available</span>
                    </div>
                </div>
            </div>
        </div>
        <div class="newproducts-banner">
            <div class="container">
                <div class="row row-cols-1 align-items-center">
                    <div class="banner-desc mb-5">
                        <h2 class="fw-semibold">In our store</h2>
                        <p class="fs-4">Chekout some of our products at the low price</p>
                        <button class="btn-lg" btn-icon="arrow-right" btn-label="Discover now" btn-url="shop">Discover now</button>
                    </div>
                    <div class="products">
                        <div class="carousel slide container" id="newProductsCarousel" data-bs-ride="carousel">
                            <div class="carousel-inner">
                                <div class="carousel-item">
                                    <div class="products-list row row-cols-1 d-flex align-items-stretch justify content">
                                        <ProductItemCard class="col-11 d-block" product-title="" product-price="$300" product-image="/assets/Chair-1.jpg"></ProductItemCard>
                                        <ProductItemCard class="col-11 d-block" product-title="" product-price="$250" product-image="/assets/Table-1.jpg"></ProductItemCard>
                                        <ProductItemCard class="col-11 d-block" product-title="" product-price="$800" product-image="/assets/Sofa-1.jpg"></ProductItemCard>
                                        <ProductItemCard class="col-11 d-block" product-title="" product-price="$400" product-image="/assets/Cabinet-1.jpg"></ProductItemCard>
                                    </div>
                                </div>
                                <div class="carousel-item">
                                    <div class="products-list row row-cols-1 d-flex align-items-stretch justify content">
                                        <ProductItemCard class="col-11 d-block" product-title="" product-price="$400" product-image="/assets/Chair-2.jpg"></ProductItemCard>
                                        <ProductItemCard class="col-11 d-block" product-title="" product-price="$350" product-image="/assets/Table-2.jpg"></ProductItemCard>
                                        <ProductItemCard class="col-11 d-block" product-title="" product-price="$500" product-image="/assets/Sofa-2.jpg"></ProductItemCard>
                                        <ProductItemCard class="col-11 d-block" product-title="" product-price="$450" product-image="/assets/Cabinet-2.jpg"></ProductItemCard>
                                    </div>
                                </div>
                                <div class="carousel-item">
                                    <div class="products-list row row-cols-1 d-flex align-items-stretch justify content">
                                        <ProductItemCard class="col-11 d-block" product-title="" product-price="$350" product-image="/assets/Chair-3.jpg"></ProductItemCard>
                                        <ProductItemCard class="col-11 d-block" product-title="" product-price="$550" product-image="/assets/Table-3.jpg"></ProductItemCard>
                                        <ProductItemCard class="col-11 d-block" product-title="" product-price="$700" product-image="/assets/Sofa-3.jpg"></ProductItemCard>
                                        <ProductItemCard class="col-11 d-block" product-title="" product-price="$560" product-image="/assets/Cabinet-3.jpg"></ProductItemCard>
                                    </div>
                                </div>
                                <div class="carousel-item">
                                    <div class="products-list row row-cols-1 d-flex align-items-stretch justify content">
                                        <ProductItemCard class="col-11 d-block" product-title="" product-price="$500" product-image="/assets/Chair-4.jpg"></ProductItemCard>
                                        <ProductItemCard class="col-11 d-block" product-title="" product-price="$600" product-image="/assets/Table-4.jpg"></ProductItemCard>
                                        <ProductItemCard class="col-11 d-block" product-title="" product-price="$750" product-image="/assets/Sofa-4.jpg"></ProductItemCard>
                                        <ProductItemCard class="col-11 d-block" product-title="" product-price="$500" product-image="/assets/Cabinet-4.jpg"></ProductItemCard>
                                    </div>
                                </div>
                            </div>
                            <span class="carousel-btn" type="button" data-bs-target="#newProductsCarousel" data-bs-slide="prev">
                                <span class="btn text-white d-flex justify-content-center align-items-center">
                                    <span class="bi bi-arrow-left"></span>
                                </span>
                            </span>
                            <span class="carousel-btn" type="button" data-bs-target="#newProductsCarousel" data-bs-slide="next">
                                <span class="btn text-white d-flex justify-content-center align-items-center">
                                    <span class="bi bi-arrow-right"></span>
                                </span>
                            </span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <br/>
        <footer></footer>
    </main>
</template>

<script>
import Home from '../views/Home.vue'
import Footer from '../views/Footer.vue'
import ProductItem from '../views/Productitem.vue'
</script>

<style>
.search {
    position: relative;

    input {
        width: 100%;
        padding: .5rem;
        border: none;
        height: 2rem;
        line-height: 2rem;
        position: relative;
        font-size: .75rem;
        border-radius: .25rem;
    }

    i {
        top: .5rem;
        right: .5rem;
        position: absolute;
    }
}

.main .mainbanner {
    margin-top: 78px;
}

.mainbanner .banner-image {
    position: relative;
}

.mainbanner .main -img {
    position: absolute;
    width: auto;
    top: -100px;
    left: -50px
}

@media only screen and (max-width: 1395px) {
    .main .mainbanner {
        margin-top: 72px;
    }
}

.icon-img {
    max-width: 30%;
    height: auto;
}

.carousel-btn {
    max-width: 45px;
}

.carousel-btn .btn {
    font-size: 20px;
    width: 40px;
    height: 40px;
    border-radius: 50%;
}

@media only screen and (max-width:1395px) {
    .mainbanner .main-banner-img {
        position: initial;
        max-width: 100%;
        top: 0px;
        margin-left: auto;
        margin-right: auto;
        height: auto;
    }
}

.newproducts-banner .carousel-item {
    padding-right: 50px;
    padding-left: 50px;
}

.banner-nav .banner-nav-item {
    padding: 0px 15px 0px 15px;
}

.banner-nav .banner-nav-item.active {
    opacity: 0.6;
}

@media only screen and (max-width:992px) {
    .products-bx .products-list div {
        margin-right: auto;
        margin-left: auto;
        width: 50%;
    }
}

</style>
