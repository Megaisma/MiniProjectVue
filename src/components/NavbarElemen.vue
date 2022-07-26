<template>
  <nav class="navbar navbar-expand-lg nv-margin sticky-top fixed-top" style="background-color: #6610f2">
    <div class="container-fluid">
      <a class="navbar-brand ms-5" href="#">
        <img :src="'https://drive.google.com/uc?export=view&id=1wLTvz-b2OSC3lqSKeoYEmZ2CKi9jvKfM'" alt="" width="60" height="50" />
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
        <div class="navbar-nav me-auto mb-2 mb-lg-0 ms-lg-4">
          <ul class="navbar-nav mr-auto">
                <li class="nav-item active">
                  <a class="nav-link hover-underline-animation text-white me-3 ms-3" href="#">Home <span class="sr-only"></span></a>
                </li>
                <li class="nav-item hover-underline-animation">
                  <a class="nav-link text-white me-3 ms-3" href="#">About</a>
                </li>
                <li class="nav-item hover-underline-animation">
                  <a class="nav-link text-white me-3 ms-3" href="#">Service</a>
                </li>
                <li class="nav-item hover-underline-animation">
                  <a class="nav-link text-white me-3 ms-3" href="#">Our Works</a>
                </li>
                <li class="nav-item hover-underline-animation">
                  <a class="nav-link text-white me-3 ms-3" href="#">Testimonials</a>
                </li>
                <li class="nav-item hover-underline-animation">
                  <a class="nav-link text-white me-3 ms-3" href="#">Contact Us</a>
                </li>
              </ul>
        </div>
      </div>
    </div>
  </nav>
</template>
<style scoped>
.nv-margin{
  margin-bottom: 20px;
}
</style>
