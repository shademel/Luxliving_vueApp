<template>
    <nav class="navbar py-3 navbar-expand-lg navbar-default bg-default nav-primary fixed-top" aria-label="Offcanvas navbar large">
      <div class="container">
        <a class="navbar-brand text-white" href="#">Trendy Timber </a>
        <button class="navbar-toggler border-0 fs-1 shadow-none" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasBasicNavbar1" aria-controls="offcanvasBasicNavbar1" aria-label="Toggle navigation">
          <span class="icon"><i class="bi bi-list"></i></span>
        </button>
  
        <div class="offcanvas offcanvas-end text-bg-dark bg-color-primary" tabindex="-1" id="offcanvasBasicNavbar1" aria-labelledby="offcanvasBasicNavbar1Label">
          <div class="offcanvas-header">
            <h5 class="offcanvas-title" id="offcanvasBasicNavbar1Label">Offcanvas</h5>
            <button type="button" class="btn-close btn-close-white" data-bs-dismiss="offcanvas" aria-label="Close"></button>
          </div>
          <div class="offcanvas-body">
            <ul class="navbar-nav justify-content-end align-items-sm-start align-items-lg-center flex-grow-1 pe-3">
              <span >
                <li class="nav-item">
                  <a :class="`nav-link fs-6` + isIndexActive(navlink)" aria-current="page" :href="`/` + navlink.url">{{
                    navlink.label }}</a>
                </li>
              </span>
              <li class="nav-item ms-lg-5">
                <a class="nav-link fs-5 visually-hidden" href="cart"><span class="icon"><i
                      class="bi bi-cart"></i></span></a>
              </li>
              <li class="nav-item p-0">
                <a class="nav-link fs-5" href="/favoriteS"><span class="icon"><i class="bi bi-heart"></i></span></a>
              </li>
              <li class="nav-item p-0 me-lg-3">
                <a class="nav-link fs-4" href="/cart"><span class="icon"><i class="bi bi-cart"></i></span></a>
              </li>
              <LinkButton btn-theme="light-btn" btn-label="Login / Register" btn-url="/register" btn-icon="person" outlined="true" class="nav-link" />
            </ul>
          </div>
        </div>
      </div>
    </nav>

  </template>

<script>

</script>

<style>

</style>