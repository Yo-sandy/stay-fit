<template>
  <div class="container-fluid">
    <div class="row">
      <nav class="navbar navbar-expand-lg navbar-light" style="background-color: #1f1f1f">
        <div class="container-fluid">
          <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav me-auto " >
              <li class="nav-item">
                <i class="far fa-clock me-2"></i>
              </li>
              <li class="nav-item">
                 <p  class="gym-time">Time : Monday-Friday (10am - 9pm)</p>
              </li>
            </ul>
            <form class="d-flex">
             <ul class="m-0 p-0">
               <li class="social-icon">
                 <i class="fab fa-facebook-f"></i>
                 <i class="fab fa-twitter"></i>
                 <i class="fab fa-instagram"></i>
               </li>
             </ul>
            </form>
          </div>
        </div>
      </nav>
      <nav class="navbar navbar-expand-lg navbar-light " style="background-color: #141313">
        <div class="container">
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" style="justify-content: space-between">
             <div class="stay-fit d-flex">
               <img src="/stay-fit.jpg" >
               <h1>STAY</h1>
               <h1 style="color: var(--iq-primary)">FIT</h1>
             </div>
            <div class="d-flex">
              <ul class="navbar-nav all-link me-auto mb-2 mb-lg-0">
                <li class="nav-item">
                  <nuxt-link class="nav-link  " to="#">Home</nuxt-link>
                </li>
                <li class="nav-item">
                  <nuxt-link class="nav-link  " to="#">About</nuxt-link>
                </li>
                <li class="nav-item">
                  <nuxt-link class="nav-link  " to="#">Cources</nuxt-link>
                </li>
                <li class="nav-item">
                  <nuxt-link class="nav-link  " to="#">Pages</nuxt-link>
                </li>
                <li class="nav-item">
                  <nuxt-link class="nav-link  " to="#">Features</nuxt-link>
                </li>
                <li class="nav-item">
                  <nuxt-link class="nav-link  " to="#">Blog</nuxt-link>
                </li>
                <li class="nav-item">
                  <nuxt-link class="nav-link  " to="#">Contact Us</nuxt-link>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
name: "my-navbar"
}
</script>

<style scoped>
.gym-time{
  color: white;
  margin: 0;
}
.fa-clock{
  color: white;
}
.social-icon i{
  color: white;
  font-size: 20px;
  margin-right: 20px;
}
.stay-fit img{
  max-width: 60px;
  border-radius: 60%;
}
.stay-fit h1{
  font-weight: bold;
  color: white;
  margin-left: 5px;
}
.all-link .nav-item a{
  color: var(--iq-white);
}
.all-link .nav-item a:hover{
  color: var(--iq-primary);
}
</style>
