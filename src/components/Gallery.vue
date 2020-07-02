<template>
  <div class="gallery container-fluid pt-5">
      <div class="container">
          <div class="row">
              <div class="col-12 pt-3 text-center">
                  <h2>GALLERY</h2>
                  <p>Take a virtual tour around our facilities we use in serving you</p>
              </div>
          </div>
          <div class="gallery__wrapper">
              <div class="gallery__card">
                  <div class="overlay"></div>
                  <img src="../assets/images/blog1.jpg" class="img-fluid" alt="">
              </div>
               <div class="gallery__card">
                  <div class="overlay"></div>
                  <img src="../assets/images/blog2.jpg" class="img-fluid" alt="">
              </div>
               <div class="gallery__card">
                  <div class="overlay"></div>
                  <img src="../assets/images/blog3.jpg" class="img-fluid" alt="">
              </div>
               <div class="gallery__card">
                  <div class="overlay"></div>
                  <img src="../assets/images/blog4.jpg" class="img-fluid" alt="">
              </div>
               <div class="gallery__card">
                  <div class="overlay"></div>
                  <img src="../assets/images/blog5.jpg" class="img-fluid" alt="">
              </div>
               <div class="gallery__card">
                  <div class="overlay"></div>
                  <img src="../assets/images/blog2.jpg" class="img-fluid" alt="">
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
.gallery{
    padding: 4rem 0;
    background: #f5f5f5;
    h2{
        font-weight: bold;
        color:#000;
        font-size: 3rem;
    }
    p{
        opacity: .9;
        font-size: .95rem;
        color:#2b2b2b;
    }
    .gallery__wrapper{
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
        grid-gap: 30px;
        margin-top: 2rem;
        .gallery__card{
            cursor: pointer;
            &:hover{
            animation-name: animate;
            animation-duration: 2s;
            animation-iteration-count: infinite;
            animation-direction: alternate;
            }
        }
    }
}
@keyframes animate {
    from{
        transform: scaleX(1);
        transition: all ease-in .5s;
    }
    to{
        transform: scaleX(1.1);
        transition: all ease-in-out .5s;
    }
}

//MEDIA QUERIES
@media only screen and (max-width: 600px){
    
    .gallery__wrapper{
        grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)) !important;
    }
}
</style>