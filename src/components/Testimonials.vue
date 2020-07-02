<template>
  <div class="testimonials">
      <div class="container">
        <div class="row">
          <div class="col-md-4">
            <h6>ABOUT COMPANY</h6>
            <h1>What our customers are saying</h1>
          </div>
          <div class="col-md-8">
            <div class="card__wrapper">
              <div class="card__content text1">
                <p>"This is the second time i have used their services and it was great again as usual. Very polite staff who genuinely seem to care about your experience. Competitive pricing matched this level of customer service. Great and i would recommend them anyday!"</p>
                <div class="img__holder d-flex pt-3">
                  <img src="../assets/images/avatar-1.png" class="avatar" alt="">
                  <div class="text2 pl-4">
                    <h6>Alexander Banfield</h6>
                    <p>Growth Officer</p>
                  </div>
                </div>
              </div>
               <div class="card__content text1">
                <p>"I received a car from a friend and the company handled everything from me. From clearance, registration and processing of driver's licence, the company did everything. One thing i particularly loved about them was that they constantly updated me on the status of thing. I'm glad"</p>
                <div class="img__holder d-flex pt-3">
                  <img src="../assets/images/avatar.png" class="avatar" alt="">
                  <div class="text2 pl-4">
                    <h6>Jonathan Auerbach</h6>
                    <p>Strategy Officer</p>
                  </div>
                </div>
              </div>
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
.testimonials{
    background: #F5F5F5;
    padding: 4rem 0;
    h6{
        font-weight: 400;
        padding-bottom: .5rem;
        font-size: .9rem;
        color: #ccc;
    }
     h1{
        color: $primary-color;
        font-weight: bold;
        font-size: 2.5rem;
        line-height: 1.3;
        text-transform: capitalize;
        padding-top: 2rem;
    }
    .card__wrapper{
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      grid-gap: 30px;
      .card__content{
        background: #fff;
        padding: 3rem 2.5rem;
        border-radius: 3px;
      }
      .text1, .text2 p{
        color: #627081;
        font-size: 1rem;
        line-height: 1.7;
        opacity: .9;
      }
      .text2{
        h6{
          font-weight: bold;
          color: $primary-color;
          opacity: .8;
        }
      }

    }
}

//MEDIA QUERIES
@media only screen and (max-width: 600px){
  h1{
    padding-bottom: 2rem;
    font-size: 2rem !important;
  }
}
</style>