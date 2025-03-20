<script setup>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
  <header>
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/shop">Shop</RouterLink>
        <RouterLink to="/contact">Contact</RouterLink>
        <RouterLink to="/login">Login</RouterLink>
        <RouterLink to="/signup">Signup</RouterLink>
        <RouterLink to="/cart">Cart</RouterLink>
      </nav>
  </header>

  <RouterView />
  <Carousel />
  <footer class="footer mt-5">
        <div class="container py-5 pb-0">
            <div class="row">
                <div class="col-12 col-md">
                    <span class="logo logo-brand">Lux Living </span>
                    <small class="d-block mb-3 text-body-secondary">2024</small>
                </div>

                <div class="col-6 text-left py-5">
                    <h3 class="fw-semibold text-light">Features</h3>
                    <ul class="text-small list-style-type: none">
                        <li><a class="text-decoration-none" href="#">Home</a></li>
                        <li><a class="text-decoration-none" href="#">About</a></li>
                        <li><a class="text-decoration-none" href="#">Contact</a></li>
                        <li><a class="text-decoration-none" href="#">Login/Signup</a></li>
                        <li><a class="text-decoration-none" href="#">Cart</a></li>
                    </ul>
                </div>
                <div class="col-6 text-center py-5">
                    <h3 class="fw-semibold text-light">About us</h3>
                    <ul class="text-small list-style-type: none">
                        <li><a class="text-decoration-none" href="#">About</a></li>
                        <li><a class="text-decoration-none" href="#">Contact</a></li>
                    </ul>
                </div>
                <div class="col-6 text-right py-5">
                    <h3 class="fw-semibold text-light">Policy & Terms</h3>
                    <ul class="text-small list-style-type: none">
                        <li><a class="text-decoration-none" href="#">Terms & Conditions</a></li>
                        <li><a class="text-decoration-none" href="#">Privacy Policy</a></li>
                        <li><a class="text-decoration-none" href="#">Our Store</a></li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
import Carousel from './views/Carousel.vue';
import footer from './views/Footer.vue';

export default {
  name: "myApp",
  components: {
    footer
  }
}

</script>

<style scoped>
#app {
  text-align: center;
  font-family: Arial, Helvetica, sans-serif;
  color: #FCF5FF;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

#nav {
  padding: 30px;
}

#nav a {
  color: #FCF5FF;
  font-weight: bold;
}

#nav a.router-link-exact-active {
  color: #FCF5FF;
}

footer {
  margin-top : 100px;
  background-color:#232F3E;
  font-size:16px;
  font-family: 'Roboto', sans-serif;
}

.footer-link {
  color: #232F3E;
}
</style>
