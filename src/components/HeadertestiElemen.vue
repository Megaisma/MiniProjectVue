<template>
    <div class="container-fluid mt-5">
        <section class="client pt-3 pb-5">
            <div class="container">
                <div class="row text-center">
                    <div class="col-12">
                        <h3 style="text-align: center; color:white; font-family: Cinzel, serif; margin-bottom: 20px;">
                            Testimonials
                        </h3>
                        <hr class="bg-white mb-4 mt-0 d-inline-block mx-auto" style="width: 100px; height:3px;">
                        <p class="p-text text-white">What our clients are saying</p>
                    </div>
                </div>
                <div class="row align-items-md-center text-white">
                    <div class="col-lg-12 col-md-12 col-sm-12">
                        <div id="carouselExampleCaptions" class="carousel slide" data-bs-ride="carousel">

                            <div class="carousel-inner" v-for="(testi, $index) in testimoni" :key="$index">
                                <div class="carousel-item active">
                                    <div class="row p-4">
                                        <div class="t-card">
                                            <i class="fa fa-quote-left" aria-hidden="true"></i>
                                            <p class="lh-lg">{{testi.message}}</p>
                                            <i class="fa fa-quote-right" aria-hidden="true"></i>

                                        </div>
                                        <div class="row">
                                            <div class="col-sm-2 pt-3">
                                                <img src="https://source.unsplash.com/300x300/?girl"
                                                    class="rounded-circle img-responsive img-fluid">
                                            </div>
                                            <div class="col-sm-10">
                                                <div class="arrow-down d-none d-lg-block"></div>
                                                <h4><strong>{{testi.name}}</strong></h4>
                                                <p class="testimonial_subtitle"><span>{{testi.designation}}</span>
                                                    <br>
                                                    <span>{{testi.location}}</span>
                                                </p>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>

                        </div>
                        <div class="controls push-right">
                            <a class="left fa fa-chevron-left text-white btn btn btn-outline-light"
                                href="#carouselExampleCaptions" data-bs-slide="prev"></a>
                            <a class="right fa fa-chevron-right text-white btn btn btn-outline-light"
                                href="#carouselExampleCaptions" data-bs-slide="next"></a>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>
<script>
export default {
  data() {
    return {
      testimoni: []
    }
  },
  mounted() {
    fetch("https://testimonialapi.toolcarton.com/api")
      .then((response) => response.json())
      .then((response) => {
        this.testimoni = response
      })
  }
}


</script>
