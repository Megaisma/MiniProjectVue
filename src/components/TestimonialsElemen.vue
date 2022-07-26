<template>
<div class="container-fluid mt-5">
<section class="client pt-3 pb-5">
  <div class="container">
    <div class="row text-center">
      <div class="col-12">
        <h3 style="text-align: center; color:white; font-family: Cinzel, serif; margin-bottom: 20px;">Testimonials</h3>
        <hr class="bg-white mb-4 mt-0 d-inline-block mx-auto" style="width: 100px; height:3px;">
        <p class="p-text text-white">What our clients are saying</p> 
      </div>
    </div>
    <div class="row align-items-md-center text-white">
      <div class="col-lg-12 col-md-12 col-sm-12">
     <div id="carouselExampleCaptions" class="carousel slide" data-bs-ride="carousel">
              <!-- Wrapper for slides -->
    <div class="carousel-inner">
      <div class="carousel-item active">
        <div class="row p-4">
          <div class="t-card">
                <i class="fa fa-quote-left" aria-hidden="true"></i>
        <p class="lh-lg">Review goes here...</p>
                      <i class="fa fa-quote-right" aria-hidden="true"></i>

                    </div>
          <div class="row">                    
           <div class="col-sm-2 pt-3">
             <img src="https://source.unsplash.com/300x300/?girl" class="rounded-circle img-responsive img-fluid">
                        </div>                    
              <div class="col-sm-10">
            <div class="arrow-down d-none d-lg-block"></div>
             <h4><strong>Sunaina Samuel</strong></h4>
        <p class="testimonial_subtitle"><span>Associate Software Engineer</span>

            <span>CodeHim</span>
                        </p>
                    </div>
                    </div>
                  </div>
                </div>
               <div class="carousel-item">
                   <div class="row p-4">
                    <div class="t-card">
                    <i class="fa fa-quote-left" aria-hidden="true"></i>
                    <p class="lh-lg">Review goes here... </p>
           <i class="fa fa-quote-right" aria-hidden="true"></i>

           </div>
        <div class="row">
         <div class="col-sm-2 pt-4">
   <img src="https://source.unsplash.com/300x300/?man" class="rounded-circle img-responsive img-fluid">
                        </div>
           <div class="col-sm-10">
            <div class="arrow-down d-none d-lg-block"></div>
             <h4><strong>Esther Zawadi</strong></h4>
        <p class="testimonial_subtitle"><span>
          digital strategist</span>

          <span>Vaxa digital</span>
                </p>
                    </div>
                    </div>
                  </div>
                </div>
               <div class="carousel-item">
                   <div class="row p-4">
                    <div class="t-card">
                    <i class="fa fa-quote-left" aria-hidden="true"></i>
                    <p class="lh-lg">Review goes here...</p>
                      <i class="fa fa-quote-right" aria-hidden="true"></i>

                    </div>
                    <div class="row text-lg-start">
                    <div class="col-sm-2 pt-4 align-items-center">
                        <img src="https://source.unsplash.com/300x300/?businessman" class="rounded-circle img-responsive img-fluid">
                        </div>
                        <div class="col-sm-10">
                          <div class="arrow-down d-none d-md-block"></div>
                        <h4><strong>Patrick muriungi</strong></h4>
                        <p class="testimonial_subtitle"><span>Web Technologist</span>

                        <span>Vaxa digital</span>
                        </p>
                    </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="controls push-right">
                <a class="left fa fa-chevron-left text-white btn btn btn-outline-light" href="#carouselExampleCaptions"
                  data-bs-slide="prev"></a>
                <a class="right fa fa-chevron-right text-white btn btn btn-outline-light" href="#carouselExampleCaptions"
                  data-bs-slide="next"></a>
              </div>
        </div>
    </div>
  </div>
  </section>
</div>
</template>
<style scoped>
.client {
    width: 100%;
    height: 100%;
    background-color: #6610f2;
}

.carousel-icon i {
  font-size: 5rem;
  color: rgba(255, 255, 255, 0.3);
}

.carousel-item i {
  font-size: 1.6rem;
  color: rgba(255, 255, 255, 0.3);
}

.t-card {
  padding: 1.8125rem 1.125rem;
  background-color: rgba(0, 0, 0, 0.5);
  border-radius: 1.25rem;
  color: #fff;
  height: auto;
}

.arrow-down {
  width: 0;
  height: 0;
  border-left: 1.5625rem solid transparent;
  border-right: 1.5625rem solid transparent;
  border-top: 1.25rem solid rgba(0, 0, 0, 0.5);
}
</style>