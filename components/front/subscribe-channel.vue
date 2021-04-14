<template>
<div class="row">
  <div class="appilo-video-box">
    <section class="home-newsletter">
      <div class="container">
        <div class="row">
          <div>
            <div class="single">
              <h2>Subscribe to our Channel</h2>
              <div class="input-group">
                <input type="email" class="form-control" placeholder="Enter your email">
                <span class="input-group-btn">
         <button class="btn btn-theme" type="submit">Subscribe</button>
         </span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</div>
</template>

<script>
export default {
  name: "subscribe-channel"
}
</script>

<style scoped>
.appilo-video-box {
  background:#d9378b url('/gym partner 2.jpg') center center no-repeat ;
  background-size:cover;
  position:relative;
  padding: 200px 5px;
}
.appilo-video-box:before {
  content:'';
  position:absolute;
  top:0;
  left:0;
  right:0;
  bottom:0;
  background:rgba(61,30,130,.67)
}
.home-newsletter {
  padding: 80px 0;

}

.home-newsletter .single {
  max-width: 650px;
  margin: 0 auto;
  text-align: center;
  position: relative;
  z-index: 2; }
.home-newsletter .single h2 {
  font-size: 25px;
  color: var(--iq-primary);
  text-transform: uppercase;
  margin-bottom: 40px; }
.home-newsletter .single .form-control {
  height: 50px;
  background: rgba(255, 255, 255, 0.6);
  border-color: transparent;
  border-radius: 20px 0 0 20px; }
.home-newsletter .single .form-control:focus {
  box-shadow: none;
  border-color: var(--iq-primary); }
.home-newsletter .single .btn {
  min-height: 50px;
  padding: 0px 30px;
  border-radius: 0 20px 20px 0;
  background: var(--iq-primary);
  color: #fff;
}
</style>
