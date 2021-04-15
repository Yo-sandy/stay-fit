<template>
<div class="send-massage">
  <div class="container size-fix" >
    <div class="row">
      <div class="services-heading " style="padding-top: 50px">
        <h2>SEND US A MASSAGE</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. </p>
      </div>
      <div class="col-md-6" style="padding-top: 130px">
        <template>
          <v-form  >
            <v-container>
              <v-row>
                <v-col
                  cols="12"
                  md="6"
                >
                  <v-text-field
                    dark
                    :counter="10"
                    label="First name"
                    required
                  ></v-text-field>
                </v-col>

                <v-col
                  cols="12"
                  md="6"
                >
                  <v-text-field
                    dark
                    :counter="10"
                    label="Last name"
                    required
                  ></v-text-field>
                </v-col>

                <v-col
                  cols="12"
                  md="6"
                >
                  <v-text-field
                    dark
                    label="E-mail"
                    required
                  ></v-text-field>
                </v-col>
                <v-col
                  cols="12"
                  md="6"
                >
                  <v-text-field
                    dark
                    :counter="7"
                    label="Phone Number"
                    required
                  ></v-text-field>
                </v-col>
                <v-text-field
                  dark
                  label="Massage" ></v-text-field>
                <v-col
                  cols="12"
                  md="2">
                  <v-btn
                    color="var(--iq-primary)"
                    class="mr-4"
                  >
                    Send Now
                  </v-btn>
                </v-col>
              </v-row>
            </v-container>
          </v-form>
        </template>
      </div>
      <div class="col-md-6 couple-img">
        <img src="/couple.png" alt="" class="img-fluid" style="max-width: 400px">
      </div>
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: "send-message"
}
</script>

<style scoped>

</style>
