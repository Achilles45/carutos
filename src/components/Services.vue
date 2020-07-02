<template>
  <div class="services" id="services">
      <div class="container">
          <div class="row">
              <div class="col-12 text-center">
                  <h6>OUR SERVICES</h6>
                  <h1>Great car service</h1>
              </div>
          </div>
          <div class="service__wrapper">
              <div class="service__card">
                  <img src="../assets/images/car2.svg" class="icons" alt="">
                  <h5>Registration</h5>
                  <p>Bought a new car or a new car has been shipped to you by a friend or relative and need urgent registration? We've got you covered as you can complete the entire registraion process online and in 24 hours or less.</p>
              </div>
               <div class="service__card">
                  <img src="../assets/images/maintainace.svg" class="icons" alt="">
                  <h5>Maintainance</h5>
                  <p>Once our auto garage launch, you will be able to get your car serviced by our professionals using latest technology at a very fair price. With this, you don't have to worry about any break down as we've got you covered.</p>
              </div>
               <div class="service__card">
                  <img src="../assets/images/car3.svg" class="icons" alt="">
                  <h5>Drivers Licence</h5>
                  <p>The company can also help you process your driver' licence effortlessly. The entire process is online and you can have your licence delivered directly to you on email or through our delivery personnels.</p>
              </div>
               <div class="service__card">
                  <img src="../assets/images/clearance.svg" class="icons" alt="">
                  <h5>Clearance.</h5>
                  <p>The company also helps in colloration with our partners at customs to make your car clearance super easy and fast and it can be completed in days. We handle all the process for you and get the car delivered to your doorstep countrywide.</p>
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
.services{
    background: linear-gradient(rgba(245, 245, 245, .8), rgba(245, 245, 245, .8)), url('../assets/images/bg-service.png');
    background-size: cover;
    background-position: center;
    padding: 5rem 0;
    h6{
        font-weight: 400;
        padding-bottom: .5rem;
        font-size: .9rem;
        color: #ccc;
    }
    h1{
        color: $primary-color;
        font-weight: bold;
        font-size: 3.4rem;
        line-height: 1.3;
        text-transform: capitalize;
    }
    .service__wrapper{
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
        grid-gap: 20px;
        margin-top: 2rem;
        .service__card{
            background: #fff;
            border-radius: 2px;
            padding: 3rem 2rem;
            text-align: center;
            .icons{
                max-width: 50px;
                height: auto;
                padding-bottom: 1rem;
                padding-top: 1rem;
            }
            h5{
                font-weight: bold;
                color: $primary-color;
                font-size: 1.2rem;
                padding-bottom: 1rem;
                padding-top: 1rem;
            }
            p{
                color: #627081;
                font-size: .87rem;
                line-height: 1.8;
            }
        }
    }
}

//MEDIA QUERIES
@media only screen and (max-width: 600px){
    h1{
        font-size: 2rem !important;
    }
}
</style>