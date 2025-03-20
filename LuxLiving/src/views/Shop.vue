<template>
    <nav></nav>
    <main>
        <div class="mainbanner">
            <div class="carousel">
                <div class="carousel-indicators">
                    <button class="active btn-indicator" type="button" data-bs-target="#mainbanner" aria-label="Slide 1"></button>
                    <button class="btn-indicator" type="button" data-bs-target="#mainbanner" aria-label="Slide 2"></button>
                    <button class="btn-indicator" type="button" data-bs-target="#mainbanner" aria-label="Slide 3"></button>
                </div>
                <div class="carousel-inner">
                    <div class="carousel-item">
                        <div class="container carousel-content d-flex justify-content-evenly align-items-stretch">
                            <div class="d-flex justify-content-center align-items-start flex-column">
                                <h1 class="display-4 fw-semibold">Chanel Mini</h1>
                                <button class="btn-lg fw-semibold" btn-label="Discover now" btn-theme="dark-btn" btn-icon="arrow-right" outlined="true"></button>
                            </div>
                            <div class="carousel-img d-flex justify-content-center align-itemes-start">
                                <img class="img img-fluid" src="../assets/Slide-image-1.jpg" alt="">
                            </div>
                        </div>
                    </div>
                    <div class="carousel-item">
                        <div class="container carousel-content d-flex justify-content-evenly align-items-stretch">
                            <div class="d-flex justify-content-center align-items-start flex-column">
                                <h1 class="display-4 fw-semibold">Modern Sofa</h1>
                                <button class="btn-lg fw-semibold" btn-label="Discover now" btn-theme="dark-btn" btn-icon="arrow-right" outlined="true"></button>
                            </div>
                            <div class="carousel-img d-flex justify-content-center align-itemes-start">
                                <img class="img" src="../assets/Slide-image-2.jpg" alt="">
                            </div>
                        </div>
                    </div>
                    <div class="carousel-item">
                        <div class="container carousel-content d-flex justify-content-evenly align-items-stretch">
                            <div class="d-flex justify-content-center align-items-start flex-column">
                                <h1 class="display-4 fw-semibold">Jaguar Frame</h1>
                                <button class="btn-lg fw-semibold" btn-label="Discover now" btn-theme="dark-btn" btn-icon="arrow-right" outlined="true"></button>
                            </div>
                            <div class="carousel-img d-flex justify-content-center align-itemes-start">
                                <img class="img" src="../assets/Slide-image-3.jpg" alt="">
                            </div>
                        </div>
                    </div>
                </div>
                <button class="carousel-control carousel-control-prev" type="button" data-bs-target="#mainbanner" data-sb-slide="prev">
                    <span class="bi bi-chevron-left" aria-hidden="true"></span>
                    <span class="visually-hidden">Previous</span>
                </button>
                <button class="carousel-control carousel-control-next" type="button" data-bs-target="#mainbanner" data-sb-slide="next">
                    <span class="bi bi-chevron-right" aria-hidden="true"></span>
                    <span class="visually-hidden">Next</span>
                </button>
            </div>
        </div>
        <br>
        <br>
        
        <div class="card" :class="layout">
            <a class="link" :href="url"></a>
            <div class="image">
                <img src="../assets/chairImages/Chair-1.jpg" :alt="imageAlt">
            </div>
            <div class="content">
                <div class="brand">{{ brand }}</div>
                <div class="title">Armchair</div>
                <div class="price">${{ 300 }}.00</div>
            </div>
            <br>
            <div class="button">
                <button @click="addToCart(product._id, 1)">Add to cart</button>
            </div>
        </div>
        <div class="card" :class="layout">
            <a class="link" :href="url"></a>
            <div class="image">
                <img src="../assets/chairImages/Chair-2.jpg" :alt="imageAlt">
            </div>
            <div class="content">
                <div class="brand">{{ brand }}</div>
                <div class="title">Wing</div>
                <div class="price">${{ 250 }}.00</div>
            </div>
            <br>
            <div class="button">
                <button @click="addToCart(product._id, 1)">Add to cart</button>
            </div>
        </div>
        <div class="card" :class="layout">
            <a class="link" :href="url"></a>
            <div class="image">
                <img src="../assets/chairImages/Chair-3.jpg" :alt="imageAlt">
            </div>
            <div class="content">
                <div class="brand">{{ brand }}</div>
                <div class="title">Chesterfield</div>
                <div class="price">${{ 150 }}.00</div>
            </div>
            <div class="button">
                <button @click="addToCart(product._id, 1)">Add to cart</button>
            </div>
        </div>
        <div class="card" :class="layout">
            <a class="link" :href="url"></a>
            <div class="image">
                <img src="../assets/chairImages/Chair-4.jpg" :alt="imageAlt">
            </div>
            <div class="content">
                <div class="brand">{{ brand }}</div>
                <div class="title">Slipper</div>
                <div class="price">${{ 100 }}.00</div>
            </div>
            <div class="button">
                <button @click="addToCart(product._id, 1)">Add to cart</button>
            </div>
        </div>
        <div class="card" :class="layout">
            <a class="link" :href="url"></a>
            <div class="image">
                <img src="../assets/cabinetImages/Cabinet-1.jpg" :alt="imageAlt">
            </div>
            <div class="content">
                <div class="brand">{{ brand }}</div>
                <div class="title">Futon</div>
                <div class="price">${{ 70 }}.00</div>
            </div>
            <div class="button">
                <button @click="addToCart(product._id, 1)">Add to cart</button>
            </div>
        </div>
        <div class="card" :class="layout">
            <a class="link" :href="url"></a>
            <div class="image">
                <img src="../assets/cabinetImages/Cabinet-2.jpg" :alt="imageAlt">
            </div>
            <div class="content">
                <div class="brand">{{ brand }}</div>
                <div class="title">Side</div>
                <div class="price">${{ 100 }}.00</div>
            </div>
            <br>
            <div class="button">
                <button @click="addToCart(product._id, 1)">Add to cart</button>
            </div>
        </div>
        <div class="card" :class="layout">
            <a class="link" :href="url"></a>
            <div class="image">
                <img src="../assets/cabinetImages/Cabinet-3.jpg" :alt="imageAlt">
            </div>
            <div class="content">
                <div class="brand">{{ brand }}</div>
                <div class="title">Cabin</div>
                <div class="price">${{ 90 }}.00</div>
            </div>
            <div class="button">
                <button @click="addToCart(product._id, 1)">Add to cart</button>
            </div>
        </div>
        <div class="card" :class="layout">
            <a class="link" :href="url"></a>
            <div class="image">
                <img src="../assets/cabinetImages/Cabinet-4.jpg" :alt="imageAlt">
            </div>
            <div class="content">
                <div class="brand">{{ brand }}</div>
                <div class="title">Console</div>
                <div class="price">${{ 95 }}.00</div>
            </div>
            <div class="button">
                <button @click="addToCart(product._id, 1)">Add to cart</button>
            </div>
        </div>
        <div class="card" :class="layout">
            <a class="link" :href="url"></a>
            <div class="image">
                <img src="../assets/sofaImages/Sofa-1.jpg" :alt="imageAlt">
            </div>
            <div class="content">
                <div class="brand">{{ brand }}</div>
                <div class="title">Lawson</div>
                <div class="price">${{ 200 }}.00</div>
            </div>
            <div class="button">
                <button @click="addToCart(product._id, 1)">Add to cart</button>
            </div>
        </div>
        <div class="card" :class="layout">
            <a class="link" :href="url"></a>
            <div class="image">
                <img src="../assets/sofaImages/Sofa-2.jpg" :alt="imageAlt">
            </div>
            <div class="content">
                <div class="brand">{{ brand }}</div>
                <div class="title">Mid-century</div>
                <div class="price">${{ 250 }}.00</div>
            </div>
            <div class="button">
                <button @click="addToCart(product._id, 1)">Add to cart</button>
            </div>
        </div>
        <div class="card" :class="layout">
            <a class="link" :href="url"></a>
            <div class="image">
                <img src="../assets/sofaImages/Sofa-3.jpg" :alt="imageAlt">
            </div>
            <div class="content">
                <div class="brand">{{ brand }}</div>
                <div class="title">Kendall</div>
                <div class="price">${{ 150 }}.00</div>
            </div>
            <div class="button">
                <button @click="addToCart(product._id, 1)">Add to cart</button>
            </div>
        </div>
        <div class="card" :class="layout">
            <a class="link" :href="url"></a>
            <div class="image">
                <img src="../assets/sofaImages/Sofa-4.jpg" :alt="imageAlt">
            </div>
            <div class="content">
                <div class="brand">{{ brand }}</div>
                <div class="title">Summer</div>
                <div class="price">${{ 270 }}.00</div>
            </div>
            <div class="button">
                <button @click="addToCart(product._id, 1)">Add to cart</button>
            </div>
        </div>
        <div class="card" :class="layout">
            <a class="link" :href="url"></a>
            <div class="image">
                <img src="../assets/tableImages/Table-1.jpg" :alt="imageAlt">
            </div>
            <div class="content">
                <div class="brand">{{ brand }}</div>
                <div class="title">Sheesham</div>
                <div class="price">${{ 140 }}.00</div>
            </div>
            <div class="button">
                <button @click="addToCart(product._id, 1)">Add to cart</button>
            </div>
        </div>
        <div class="card" :class="layout">
            <a class="link" :href="url"></a>
            <div class="image">
                <img src="../assets/tableImages/Table-2.jpg" :alt="imageAlt">
            </div>
            <div class="content">
                <div class="brand">{{ brand }}</div>
                <div class="title">Modern</div>
                <div class="price">${{ 180 }}.00</div>
            </div>
            <div class="button">
                <button @click="addToCart(product._id, 1)">Add to cart</button>
            </div>
        </div>
        <div class="card" :class="layout">
            <a class="link" :href="url"></a>
            <div class="image">
                <img src="../assets/tableImages/Table-3.jpg" :alt="imageAlt">
            </div>
            <div class="content">
                <div class="brand">{{ brand }}</div>
                <div class="title">Century</div>
                <div class="price">${{ 120 }}.00</div>
            </div>
            <div class="button">
                <button @click="addToCart(product._id, 1)">Add to cart</button>
            </div>
        </div>
        <div class="card" :class="layout">
            <a class="link" :href="url"></a>
            <div class="image">
                <img src="../assets/tableImages/Table-4.jpg" :alt="imageAlt">
            </div>
            <div class="content">
                <div class="brand">{{ brand }}</div>
                <div class="title">Parsons</div>
                <div class="price">${{ 90 }}.00</div>
            </div>
            <div class="button">
                <button @click="addToCart(product._id, 1)">Add to cart</button>
            </div>
        </div>
    </main>
</template>

<script>
export default {
    name: 'Shop',
    props: {
        id: String,
        image: String,
        imageAlt: String,
        brand: String,
        title: String, 
        price: String,
        url: String,
        layout: String
    },
    computed: {
        hasURL () {
            return !!this.$props['url']
        },
        hasImage () {
            return !!this.$props['image']
        }
    }
}
</script>

<style>
#mainbanner .carousel-img .img {
    height: auto;
    width: 100%;
    max-width: 100%;
}

#mainbanner .carousel-indicators .btn-indicator {
    height: 15px;
    width: 15px;
    margin: 8px;
    background-color: #265a5a;
    border-radius: 50%;
}

.mainbanner .carousel-control {
    opacity: 1.0;
    width: auto;
}

.carousel-item .btn-lg,
.btnLight {
    font-size: 18px;
    border: 0px;
}

.mainbanner .carousel-control .bi {
    display: block;
    color: #0c0c0c;
    font-size: 40px;
}

.mainbanner .carousel-img {
    position: relative;
}

.mainbanner .carousel-img::after {
    opacity: 0.2;
    width: 400px;
    height: 400px;
    top: 0;
    left: 0;
    z-index: 1;
    transform: translate(15%, 38%);
    position: absolute;
    border-radius: 50%;
}

.mainbanner .carousel-img img {
    z-index: 2;
}

.newproducts-banner .carousel-item {
    padding-right: 40px;
    padding-left: 40px;
}

.newproducts-banner .carousel-control-prev.btn {
    left: -19%;
    position: absolute;
}

.newproducts-banner .carousel-control-next.btn {
    right: -19%;
    position: absolute;
}
.newproducts-banner .carousel-btn .btn {
    font-size: 20px;
    height: 40px;
    width: 40px;
    border-radius: 50%;
}

.newproducts-banner .carousel-control-prev,
.newproducts-banner .carousel-control-next {
    max-width: 40px;
}

.card {
    width: 100%;
    position: relative;
    border-radius: .25rem;
    display: flex;


    img {
        height: auto;
        width: 100%;
    }

    .brand {
        margin: 1rem 0 0;
        font-size: .75rem;
    }

    .title {
        font-weight: 700;
        font-size: .875rem;
    }

    .price {
        font-size: 1.25rem;
        margin-bottom: 0;
        font-weight: 700;
    }

    &.list {
        align-items: center;
        padding: 0;
        flex-direction: row;

        .image {
            text-align: center;
            height: 100%;
            padding: .75rem;
        }
        .brand {
            margin-top: 0;
        }

        .content {
            padding: .75rem;
        }
    }

    .button {
        text-align: center;
        cursor: pointer;
        border: none;
        outline: 0;
        width: 100%;
        font-size: 18px;
        padding: 12px;
    }
}
</style>