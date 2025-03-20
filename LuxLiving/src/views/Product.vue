<template>
    <br>
    <div class="container">
        <h1>Products</h1>
        <div class="container-fluid">
            <div class="row row-cols-1">
                <div class="col hp">
                    <div class="card1 shadow-sm">
                        <a href="#">
                            <img class="card1-img-top" alt="product.title">
                        </a>
                        <div class="label-top">
                            <a class="text-white" href="#">{{ item.brand }}</a>
                        </div>
                        <div class="card-body">
                            <div class="mb-3">
                                <span class="float-start">{{ item.price }}</span>
                            </div>
                            <h4 class="card-title">
                                <a @click="GoToDetails(item.name)">{{ item.description }}</a>
                            </h4>
                            <div class="gap-2 my-4">
                                <button @click="
                                addToCart(item),
                                  getData(
                                    item.name,
                                    item.brand,
                                    item.price,
                                    item.description,
                                    item.image,
                                    item.key
                                  )" class="btn btn-warning">Add to cart</button>
                            </div>
                            <div class="mb-1">
                                <span class="float-start"><a href="#"><i class="fa-question-circle"></i></a></span>
                                <span class="float-end">
                                    <i class="fa-heart" style="cursor: pointer"></i>
                                </span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="justify-content-center d-flex">
                <div class="border">
                    <span class="sr-only">Loading..</span>
                </div>
            </div>
        </div>
        <nav>
            <ul class="justify-content-center">
                <li class="page-item" @click="Previous">
                    <a class="page-link" href="#"></a>
                </li>
                <li class="page-item" @click="Next">
                    <a class="page-link" href="#"></a>
                </li>
            </ul>
        </nav>
    </div>
    <div class="modal fade">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <div>
                        <img src="../assets/chaiImages/chair-1.jpg">
                        <h4 class="modal-title">Product added to cart</h4>
                    </div>
                </div>
                <div class="modal-body">
                    <div class="card mb-3">
                        <div class="row">
                            <div class="col-md-4">
                                <img class="img-fluid">
                            </div>
                            <div class="col-md-8">
                                <div class="card-body">
                                    <h4 class="card-title">{{ dataProduct.name }}</h4>
                                    <h5 class="card-text">{{ dataProduct.brand }}</h5>
                                    <br>
                                    <h5 class="card-text">Price: {{ dataProduct.price }}</h5>
                                    <p class="card-text">There are {{ $store.state.count }} items in your cart</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>

</script>

<style>

</style>