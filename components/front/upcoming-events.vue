<template>
  <div class="row">
    <div class="our-services-section">
      <div class="services-heading">
        <h2>UPCOMING EVENTS</h2>
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
                  <div class="card b">
                    <span></span>
                    <div class="content">
                      <h2>Card One</h2>
                      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quia aliquid harum !</p>
                      <button class="btn btn-join" style="background-color: var(--iq-primary);">
                         Read More
                      </button>
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
.card {
  position: relative;
  border: none;
  background-color: #1e1d1d;
  width: 320px;
  height: 400px;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 40px 0px;
  transition: 0.4s;
}

.card::before {
  content: "";
  position: absolute;
  width: 50%;
  height: 100%;
  top: 0;
  left: 50px;
  border-radius: 10px;
  transform: skewx(15deg);
  transition: 0.4s;
}

.card::after {
  content: "";
  position: absolute;
  width: 50%;
  height: 100%;
  top: 0;
  left: 50px;
  border-radius: 10px;
  transform: skewx(15deg);
  transition: 0.4s;

}

.card:hover::before,
.card:hover::after {
  transform: skewx(0);
  left: 20px;
  width: calc(100% - 80px);
}

.card:nth-child(1)::before,
.card:nth-child(1)::after {
  background-image: url("/All-Nighter-Work-Out.jpg");
  background-size: cover;
}



.card span {
  display: block;
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 2;
  pointer-events: none;
}

.card span::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border-radius: 10px;
  opacity: 0;
  transition: 0.4s;
}

.card:hover span::before {
  width: 100px;
  height: 100px;
  opacity: 1;
  left: 50px;
  top: -50px;
  animation: swing 2s ease-in-out infinite;
}



.card:hover span::after {
  width: 100px;
  height: 100px;
  opacity: 1;
  right: 50px;
  bottom: -50px;
  animation: swing 2s ease-in-out infinite;
  animation-delay: -1s;
}

.content {
  z-index: 1;
  position: relative;
  left: 0;
  border-radius: 10px;
  padding: 20px 50px;
  transition: 0.4s;
  color: white;
}

.card:hover .content {
  left: -25px;
  padding: 40px 50px;
}

.card h2 {
  font-size: 1.9em;
  margin-bottom: 10px;
}

.card p {
  font-size: 0.95em;
  font-weight: 300;
  margin-bottom: 20px;
}



@keyframes swing {
  0% {
    transform: translatey(10px);
  }

  50% {
    transform: translatey(-10px);
  }

  100% {
    transform: translatey(10px);
  }
}

</style>
