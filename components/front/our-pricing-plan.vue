<template>
  <section>
    <div  >
      <div class="container"  style="max-width: 1200px">
        <div class="row">
          <div class="col-sm-4">
            <div class="card card_red text-center">
              <div class="title">
                <h2>Month</h2>
              </div>
              <div class="price">
                <h4><sup>$</sup>8</h4>
              </div>
              <div class="option">
                <ul>
                  <li> 10 GB Space</li>
                  <li> 3 Domain Names</li>
                  <li> 20 Emails Address</li>
                  <li> >Live Support</li>
                </ul>
              </div>
              <a href="#">Order Now</a>
            </div>
          </div>
          <div class="col-sm-4">
            <div class="card card_violet text-center">
              <div class="title">
                <h2>Month</h2>
              </div>
              <div class="price">
                <h4><sup>$</sup>25</h4>
              </div>
              <div class="option">
                <ul>
                  <li> 10 GB Space</li>
                  <li> 3 Domain Names</li>
                  <li> 20 Emails Addresse</li>
                  <li> Live Support</li>
                </ul>
              </div>
              <a href="#">Order Now</a>
            </div>
          </div>
          <div class="col-sm-4">
            <div class="card card_three text-center">
              <div class="title">
                <h2>Month</h2>
              </div>
              <div class="price">
                <h4><sup>$</sup>50</h4>
              </div>
              <div class="option">
                <ul>
                  <li> 50 GB Space</li>
                  <li> 5 Domain Names</li>
                  <li> 20 Emails Addresse</li>
                  <li> Live Support</li>
                </ul>
              </div>
              <a href="#">Order Now</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "our-pricing-plan"
}
</script>

<style scoped>


section {
  padding: 140px 0;

}

.card {
  position: relative;
  min-width: 250px;
  height: auto;
  overflow: hidden;
  border-radius: 15px;
  margin: 0 auto;
  padding: 40px 20px;
  box-shadow: 0 10px 15px rgba(0,0,0,0.3);
  transition: .5s;
}
.card:hover {
  transform:scale(1.1);
  border: 1px solid var(--iq-primary);
}
.card_red, .card_red .title  {
  background: #1e1d1d;
}
.card_violet, .card_violet .title  {
  background: #1e1d1d;
}
.card_three, .card_three .title {
  background: #1e1d1d;
}

.card:before {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 40%;
  background: rgba(255, 255, 255, .1);
  z-index: 1;
  transform: skewY(-5deg) scale(1.5);
}


.title h2 {
  position: relative;
  margin: 20px 0 0;
  padding: 0;
  color: #fff;
  font-size: 28px;
  z-index: 2;
}
.price {
  position: relative;
  z-index: 2;
}
.price h4 {
  margin: 0;
  padding: 20px 0;
  color: #fff;
  font-size: 60px;
}
.option {
  position: relative;
  z-index: 2;
}
.option ul {
  margin: 0;
  padding: 0;
}
.option ul li {
  margin: 0 0 10px;
  padding: 0;
  list-style: none;
  color: #fff;
  font-size: 16px;
}
.card a {
  display: block;
  position: relative;
  z-index: 2;
  background-color: #fff;
  width: 150px;
  height: 40px;
  text-align: center;
  margin: 20px auto 0;
  line-height: 40px;
  border-radius: 40px;
  font-size: 16px;
  cursor: pointer;
  text-decoration: none;
  box-shadow: 0 5px 10px rgba(0,0,0, .1);
}
.card a:hover {

}
</style>
