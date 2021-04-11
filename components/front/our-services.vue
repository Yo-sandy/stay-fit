<template>
<div class="row">
    <div class="our-services-section">
      <div class="services-heading">
        <h2>OUR SERVICES</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. </p>
      </div>
      <div class="container-fluid">
        <template>
          <v-sheet
            class=" mx-auto sheet-body "
          >
            <v-slide-group
              v-model="model"
              center-active
              show-arrows
            >
              <v-slide-item
                v-for="n in 4"
                :key="n"
                v-slot="{ active, toggle }"
              >
                    <v-card
                      color="red"
                      class="pa-8"
                      @click="toggle">
                      <div>
                        <img src="/muscular-bodybuilder-grey-background-151364145.jpg"
                             class="card-img-top img-fluid"/>
                      </div>
                      <div class="text-center mt-2 text-white p-3">
                        <h4>Personal Training</h4>
                        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Architecto ducimus eaque </p>
                      </div>
                    </v-card>
              </v-slide-item>
            </v-slide-group>
          </v-sheet>
        </template>
      </div>
    </div>
</div>
</template>

<script>
export default {
  data: () => ({
    model: null,
  }),
}
</script>

<style scoped>

</style>
