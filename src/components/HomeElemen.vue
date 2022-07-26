<template>
    <div class="container-fluid nv-margin">
                <div id="carouselExampleControls" class="carousel slide" data-bs-ride="carousel">
                    <div class="carousel-inner">
                      <div class="carousel-item active">
                        <img :src="'https://drive.google.com/uc?export=view&id=1zTucY4CXuivkKNPPL73cy3CsOvzQx-qp'" class="d-block w-100" alt="First Banner">
                      </div>
                      <div class="carousel-item">
                        <img :src="'https://drive.google.com/uc?export=view&id=1ckmaMWKlwAHyVNmguwB4T6xjvRL_wK8n'" class="d-block w-100" alt="Second Banner">
                      </div>
                    </div>
                    <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="prev">
                      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                      <span class="visually-hidden">Previous</span>
                    </button>
                    <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="next">
                      <span class="carousel-control-next-icon" aria-hidden="true"></span>
                      <span class="visually-hidden">Next</span>
                    </button>
                  </div>
            </div>
</template>
<style scoped>
.nv-margin{
  margin-bottom: 25px;
}
</style>