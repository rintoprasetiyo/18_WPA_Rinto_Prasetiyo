<template>
    <!-- ======= Portfolio Section ======= -->
    <section id="portfolio" class="portfolio" data-aos="fade-up">

      <div class="container">

        <div class="section-header">
          <h2>Portofolio</h2>
        </div>

      </div>

      <div class="container-fluid" data-aos="fade-up" data-aos-delay="200">

        <div class="portfolio-isotope" data-portfolio-filter="*" data-portfolio-layout="masonry" data-portfolio-sort="original-order">

          <div class="row g-0 portfolio-container">

            <div v-for="(portofolio, $index) in folio" :key="$index" class="col-xl-3 col-lg-4 col-md-6 portfolio-item filter-app">
              <img :src="'assets/img/portfolio/'+portofolio.sumber" class="img-fluid" alt="">
              <div class="portfolio-info">
                <h4>{{portofolio.judul}}</h4>
              </div>
            </div><!-- End Portfolio Item -->

          </div><!-- End Portfolio Container -->

        </div>

      </div>
    </section><!-- End Portfolio Section -->
</template>

<script>
export default {
  data() {
    return{
      folio:[]
    }
  },
  mounted(){
    fetch("/portofolio.json")
    .then(res => res.json())
    .then(res => {
      this.folio = res
    })
  }
}
</script>