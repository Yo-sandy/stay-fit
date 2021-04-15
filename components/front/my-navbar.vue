<template>
  <div class="container-fluid px-md-5  my-navbar"  >
    <div class="row">
      <nav class="navbar navbar-expand-lg navbar-light ">
        <div>
          <div class="stay-fit d-flex">
            <h1>STAY</h1>
            <h1 style="color: var(--iq-primary)">FIT</h1>
          </div>
        </div>
        <button
          class="navbar-toggler navbar-expand-md text-white"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarSupportedContent">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav all-link me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <nuxt-link class="nav-link text-center " to="#">Home</nuxt-link>
            </li>
            <li class="nav-item">
              <nuxt-link class="nav-link text-center " to="#">About</nuxt-link>
            </li>
            <li class="nav-item">
              <nuxt-link class="nav-link text-center " to="#">Cources</nuxt-link>
            </li>
            <li class="nav-item">
              <nuxt-link class="nav-link text-center " to="#">Pages</nuxt-link>
            </li>
            <li class="nav-item">
              <nuxt-link class="nav-link text-center " to="#">Features</nuxt-link>
            </li>
            <li class="nav-item">
              <nuxt-link class="nav-link text-center " to="#">Blog</nuxt-link>
            </li>
            <li class="nav-item">
              <nuxt-link class="nav-link text-center " to="#">Contact Us</nuxt-link>
            </li>
          </ul>
        </div>
        <div class="d-none d-md-block">
          <ul class="list-unstyled d-flex">
            <li>
              <i class="far fa-clock me-2"></i>
            </li>
            <li >
              <p  class="gym-time">Time : Monday-Friday (10am - 9pm)</p>
            </li>
          </ul>
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
