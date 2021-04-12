<template>
  <div class="bg-color">
    <div class="container">
      <div class="row">
        <div class="our-classes-title">
            <h2 >Our Classes</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        </div>
        <div>
          <div class="classes-img text-center">
            <LazyYoutube src="https://www.youtube.com/watch?v=qVPCGH9EZ0U"
                         aspectRatio="16:9"
                         maxWidth="1000px"/>
        </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { LazyYoutube, } from "vue-lazytube";
export default {
  name: "our-classes",
  components: {
    LazyYoutube,
  },
}
</script>

<style scoped>

</style>
