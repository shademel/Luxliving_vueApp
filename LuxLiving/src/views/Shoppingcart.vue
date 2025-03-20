<template>
    <nav></nav>
    <main>
        <div class="container py-4">
            <div class="row py-lg-4">
                <div class="col-lg-6 col-md-8 mx-auto">
                  <h1 class="fw-bold display-5 opacity-80">My shopping cart</h1>
                </div>
            </div>
        </div>
        <div class="container col-lg-10 col-sm-11 my-5 py-5">
            <div class="row mt-3 text-center py-1 border-bottom border-black">
                <div class="col-sm-2 fw-semibold p-3 themed-grid-col">Image</div>
                <div class="col-sm-2 fw-semibold p-3 themed-grid-col">Product</div>
                <div class="col-sm-2 fw-semibold p-3 themed-grid-col">Price</div>
                <div class="col-sm-2 fw-semibold p-3 themed-grid-col">Quantity</div>
                <div class="col-sm-2 fw-semibold p-3 themed-grid-col">Total</div>
                <div class="col-sm-2 fw-semibold p-3 themed-grid-col">Delete</div>
            </div>
            <div>
                <div class="product-item row text-center border-bottom d-flex align-items-stretch justify-content-between">
                    <div class="col-sm-2 fw-semibold p-3 themed-grid-col d-flex justify-content-center align-items-center">
                        <img src="../assets/chairImages/Chair-3.jpg" class="card-img" alt="Product-img">
                    </div>
                    <div class="col-sm-2 fw-semibold p-3 themed-grid-col d-flex justify-content-center align-items-center">
                        Chair-product {{ item }}</div>
                    <div class="col-sm-2 fw-semibold p-3 themed-grid-col d-flex justify-content-center align-items-center">
                        $150
                    </div>
                    <div class="col-sm-2 fw-semibold p-3 themed-grid-col d-flex justify-content-center align-items-center">
                        <div class="d-flex justify-content-between align-items-stretch gap-1">
                            <input type="text" name="" class="form-control" value="1" id="">
                            <button class="btn btn-light border" type="button"><span class="bi bi-plus-lg"></span></button>
                            <button class="btn btn-light border" type="button"><span class="bi bi-dash-lg"></span></button>
                        </div>
                    </div>
                    <div class="col-sm-2 fw-semibold p-3 themed-grid-col d-flex justify-content-center align-items-center">
                        <span class="cursor-p bi bi-trash3 fs-4"></span>
                    </div>
                </div>
            </div>
            <div class="content-footer mt-5 pt-3">
                <div class="row d-flex justify-content-between ">
                    <div class="cart-btn col-lg-5">
                        <div class="btns-bx d-flex justify-content-center gap-2 align-items-center w-100 cart-bx-content my-3 my-lg-1">
                            <button class="rounded rounded-0 py-2 fw-semibold my-3 btn btn-light border border-1 bg-body-tertiary d-flex justify-content-center gap-2 align-items-center w-100" type="button">
                                <span class="me-2">Clear Cart</span>
                                <span class="bi bi-trash3"></span>
                            </button>
                            <LinkButton btn-theme="dark-btn" btn-label="Continue Shopping" btn-url="" btn-icon="cart-check" outlined="false" class="py-2 btn-lg my-3 w-100" />
                        </div>
                    </div>
                    <div class="cart-total col-lg-6">
                        <h2 class="fw-bold display-6 opacity-80 mb-3 border-bottom">Cart Total</h2>
                        <div class="py-1 d-flex gap-2 w-100 justify-content-between">
                            <span class="label me-5 fw-semibold">
                                No. Products
                            </span>
                            <span class="label fw-bold text-nowrap">2</span>
                        </div>
                        <div class="py-1 d-flex gap-2 w-100 justify-content-between">
                            <span class="label me-5 fw-semibold">
                                Total Price
                            </span>
                            <span class="label fw-bold text-nowrap">$300</span>
                        </div>
                        <LinkButton btn-theme="dark-btn" btn-label="Proceed To Checkout" btn-url="" btn-icon="arrow-right" outlined="false" class="btn-lg mt-3 w-100" />
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>

<script>
export default {
    name: "ShoppingCart",
    methods: {
        setPageTitle() {
            document.title = "Shopping Cart Lux Living";
        }
    },
    beforeMount() {
        this.setPageTitle()
    }
}
</script>

<style scoped>
.navbar,
.mainbanner {
    background-color: #f1f1f1 !important;
}

.card-img{
    height: auto;
    width: 100%;
}
</style>