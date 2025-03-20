<template>
    <nav></nav>
    <main>
        <section class="bg-banner text-center">
            <div class="banner-img">
                <img src="../assets/Contactus.jpg" alt="">
            </div>
            <div class="banner-blur"></div>
            <div class="container">
                <div class="row">
                    <div class="col-lg-6 col-md-8">
                        <h1 class="fw-bold text-white">Contact us</h1>
                    </div>
                </div>
            </div>
        </section>
        <section class="">
            <div class="container">
                <div class="rounded-3 bg-light">
                    <div class="text-center">
                        <div class="rounded-3 text-white"><i class="bi bi-envelope"></i></div>
                        <h1>Get in touch</h1>
                        <p class="text-muted">We love to hear from you</p>
                    </div>
                    <div class="justify-content-center">
                        <div class="col-lg-8">
                            <form id="contactForm" class="needs-validation" method="post">
                                <input name="access_key" type="hidden">
                                <input name="subject" type="hidden">
                                <input name="botcheck" type="checkbox" style="display: none;">

                                <div class="form-floating">
                                    <input type="text" id="name" class="form-control" placeholder="Enter your name " data-sb-validations="required">
                                    <label></label>
                                </div>
                                <div class="form-floating">
                                    <input type="email" id="email" class="form-control" placeholder="name@example.com " data-sb-validations="required,email">
                                    <label></label>
                                    <div class="invalid-feedback" data-sb-feedback="email:required"></div>
                                    <div class="invalid-feedback" data-sb-feedback="email:email"></div>
                                </div>
                                <div>
                                    <input class="form-control" data-sb-validations="required" name="phone" type="text" id="phone" placeholder="+61 --- --- ---">
                                    <label for="phone"></label>
                                    <div class="invalid-feedback" data-sb-feedback="phone:required"></div>
                                </div>
                                <div class="form-floating">
                                    <textarea class="form-control" type="text" id="message" placeholder="Enter your message..." data-sb-validations="required"></textarea>
                                    <label for="message"></label>
                                    <div class="invalid-feedback" data-sb-feedback="message:required"></div>
                                </div>
                                <div class="d-none" id="submitSuccessMessage">
                                    <div class="text-center">
                                        <div class="fw-bolder"></div>
                                    </div>
                                </div>
                                <div class="d-none" id="submitErrorMessage">
                                    <div class="text-center"></div>
                                </div>
                                <div class="d-grid">
                                    <button class="btn btn-success" type="submit" id="submitButton">Submit</button>
                                </div>
                            </form>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>
</template>

<script>

</script>

<style>
.navbar,
.mainbanner {
    background-color: #f1f1f1;
}

.bg-banner {
    overflow: hidden;
    position: relative;
}

.feature {
    width: 3rem;
    height: 3rem;
    display: inline-flex;
    align-items: center;
    justify-content: center;
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

button {
  background-color: #7293bf;
  color: white;
  padding: 14px 20px;
  margin: 8px 0;
  border: none;
  cursor: pointer;
  width: 100%;
}

button:hover {
  opacity: 0.8;
}

.submitbtn {
  width: auto;
  padding: 10px 18px;
  background-color: #04AA6D;
}
</style>