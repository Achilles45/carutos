<template>
  <div class="features">
      <div class="container">
          <div class="row">
              <div class="col-12">
                  <h6>EXPLORE FEATURES</h6>
                  <h1>Quality and perfomance</h1>
              </div>
          </div>
          <div class="card__wrapper">
              <div class="card__content d-flex align-items-center">
                  <img src="../assets/images/car.svg" class="icons" alt="">
                  <div class="content">
                      <h3>Customer Centric</h3>
                      <p>All of our services are designed with our customers in mind. Customer's satisfaction is at the core of all our operations.</p>
                  </div>
              </div>
              <div class="card__content d-flex align-items-center">
                  <img src="../assets/images/quality.svg" class="icons" alt="">
                  <div class="content">
                      <h3>Quality Services</h3>
                      <p>Everyone at the company is a professional and an expert in what they do, so you are sure of getting qulaity services.</p>
                  </div>
              </div>
              <div class="card__content d-flex align-items-center">
                  <img src="../assets/images/delivery.svg" class="icons" alt="">
                  <div class="content">
                      <h3>Timely Delivery</h3>
                      <p>We know how valuable time is and we don't waste your time at all. Our customers loves for for our timely delivery of our services. No stories!</p>
                  </div>
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
.features{
    padding: 4rem 0;
    background: #F5F5F5;
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
    .card__wrapper{
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
        grid-gap: 30px;
        // margin-top: 2rem;
        .card__content{
            .icons{
                max-width: 60px;
                height: auto;
                margin-right: 1rem;
            }
            .content{
                h3{
                    padding-top: 6rem;
                    font-size: 1.3rem;
                    text-transform: capitalize;
                    font-weight: bold;
                    color: $primary-color;
                    padding-bottom: .5rem;
                }
                p{
                    color: $primary-color;
                    line-height: 1.7;
                    font-size: 1rem;
                    color: #627081;
                }
            }
        }
    }
}

//MEDIA QUERIES
@media only screen and (max-width: 600px){
    .features{
        padding: 2rem 0 !important;
        h1{
        font-size: 2.5rem !important;
        padding-bottom: 2rem !important;
    }
    p{
        padding-top: 1rem !important;
    }
    .content{
        h3{
            padding-top: 1rem !important;
        }
    }
    }
}
</style>