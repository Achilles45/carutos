<template>
  <div class="intro" id="about">
      <div class="container">
          <div class="row">
              <div class="col-12">
                  <h6>ABOUT COMPANY</h6>
                  <h2>We are qualified & of experience <br> in this field</h2>
                  <p>We help you handle everything that relates to your car so you don't have to worry about anything. From car registration, drivers licence, we help you prepare all car paper works. The company is also launching out an auto garage center to provide top notch services in repairs and maintanance.</p>
                  <img src="../assets/images/img7.jpg" class="img-fluid" alt="">
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
.intro{
    background: #F5F5F5;
    padding: 4rem 0 !important;
    h6{
        font-weight: 400;
        padding-bottom: .5rem;
        font-size: .9rem;
        color: #ccc;
    }
    h2{
        color: $primary-color;
        font-weight: bold;
        font-size: 3.4rem;
        padding-bottom: 1rem;
        line-height: 1.3;
        text-transform: capitalize;
    }
    p{
        color: $primary-color;
        font-weight: 400;
        line-height: 1.7;
        padding-bottom: 2rem;
    }
}

//MEDIA QUERIES
@media only screen and (max-width: 600px){
    h2{
        font-size: 2rem !important;
    }
    p{
        padding-top: 1rem !important;
    }
}
</style>