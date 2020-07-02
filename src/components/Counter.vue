<template>
  <div class="counter">
      <div class="container">
          <div class="row">
              <div class="col-md-6 heading">
                  <h6>STATISTICS</h6>
                  <h1>Learn more about our success</h1>
              </div>
          </div>
          <div class="row text-center">
              <div class="col-md-4">
                  <i class="fa fa-car icons"></i>
                  <h2>500+ projects</h2>
              </div>
              <div class="col-md-4">
                  <i class="fas fa-funnel-dollar icons"></i>
                  <h2>$500,000+ credit</h2>
              </div>
              <!-- <div class="col-md-3">
                 <i class="fas fa-hand-holding-usd icons"></i>
                  <h3>Over &#8358;70,000,000.00 Paid to Investors</h3>
              </div> -->
              <div class="col-md-4">
                 <i class="fa fa-cubes icons"></i>
                  <h2>100+ staff</h2>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import '../assets/styles/_colors';
.counter{
    background: linear-gradient(rgba(4,9,30,.5),rgba(4,9,30,.5)), url('../assets/images/img4.jpg');
    background-size: cover;
    background-position: center;
    padding: 5rem 0;
    color: #fff;
    .icons{
        color: $secondary-color;
        font-size: 3rem;
    }
    .heading{
        h1{
            color: #fff;
            padding-bottom: 4rem;
            padding-top: 1rem;
            font-weight: 800;
            font-size: 3rem;
            line-height: 1.3;
            text-transform: capitalize;
        }
          h6{
        font-weight: 400;
        padding-bottom: .5rem;
        font-size: .9rem;
        color: #ccc;
        opacity: .7;
    }
    }
    p{
        font-size: .9rem;
        opacity: .8;
        padding-bottom: 5rem;
    }
    h2{
        padding-top: 1.5rem;
        font-weight: bold;
        font-size: 1.4rem;
        line-height: 1.5;
        opacity: .8;
    }
    h1{
        font-weight: bold;
    }
}

//MEDIA QUERIES
@media only screen and (max-width: 600px){
    h1{
        font-size: 2rem !important;
    }
}
</style>