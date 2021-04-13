<template>
<div class="row">
    <div class="our-services-section">
      <div class="services-heading">
        <h2>OUR SERVICES</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. </p>
      </div>
        <div >
          <v-sheet
               class="container"
               max-width="1100"
              color="#1e1d1d">
            <vueper-slides
              :visible-slides="3"
              slide-multiple
              :breakpoints="{ 900: { visibleSlides: 1, slideMultiple: 1, gap:0 },1200: { visibleSlides: 2, slideMultiple: 2  } }"
              :bullets="false"
              fixedHeight="400px">
              <template v-slot:arrow-left>
                <i class="fas fa-chevron-left text-white"></i>
              </template>
              <template v-slot:arrow-right>
                <i class="fas fa-chevron-right  text-white"></i>
              </template>
              <vueper-slide v-for="i in 9" :key="i" class=""  >
                <template v-slot:content>
                  <div class="vueperslide__content-wrapper ">
                    <div class="our-service-card">
                      <img src="/muscular-bodybuilder-grey-background-151364145.jpg"
                           class="our-service-img img-fluid"/>
                      <div class="text-center mt-2 text-white ">
                        <h4>Personal Training</h4>
                        <p>Lorem ipsum dolor sit amet, consec   adipisi  elit. Architecto ducimus eaque </p>
                      </div>
                    </div>
                  </div>
                </template>
              </vueper-slide>
            </vueper-slides>
          </v-sheet>
        </div>

    </div>
</div>
</template>

<script>
import { VueperSlides, VueperSlide } from 'vueperslides';
export default {
  components: { VueperSlides, VueperSlide },
  data(){
    return {
    }
  },
}
</script>

<style scoped>

</style>
