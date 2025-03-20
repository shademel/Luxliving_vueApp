<template>
    <div class="product-card">
        <div class="card-img">
            <span class="d-flex justify-content-center align-items-center">
                <button class="btn btn-success d-flex justify-content-center align-items-center" type="button"><span class="d-block bi bi-plus"></span></button>
                <span class="text-white d-block">Add to cart</span>
            </span>
            <div class="cover"></div>
            <img :src="productImage" alt="">
        </div>
        <a href="">
            <div class="card-body d-flex flex-column justify-content align-items-between">
                <span class="product-infor d-flex justify-content-between align-items-center">
                    <span class="product-category">{{ productCategory }}</span>
                </span>
                <span class="product-name fw-semibold">{{ productTitle }}</span>
                <span class="product-price">
                    <span class="fw-bold">{{ productPrice }}</span>
                </span>
            </div>
        </a>
    </div>
</template>

<script>

export default {
    name: "productitem",
    data() {
        return {

        }
    },
    props: {
        productTitle: { type: String, default: "Product title" },
        productCategory: { type: String, default: "Category" },
        productPrice: { type: String, default: "100" },
        productImage: { type: String, default: "../src/assets/Cabinet-1.jpg" }
        
    }  
}
</script>

<style>
.product-card {
    position:relative;
}

.product-card:hover .cover {
    transition: 0.5s;
    width: 100%;
    height: 100%;
    position: absolute;
}

.product-card .card-img {
    position: relative;
    overflow: hidden;
    width: 100%;
    max-height: 100%;
}

.product-card .card-img img {
    object-fit: cover;
    height: auto;
    width: 100%;
    max-height: 100%;
}
</style>