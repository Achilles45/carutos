<template>
  <div class="main__wrapper">
    <div class="home">
    <div class="container">
      <!--Topbar section begins here ========-->
      <div class="topbar d-none d-lg-block">
        <div class="row">
          <!-- <div class="col-md-2"></div> -->
          <div class="col-md-4 d-flex col-sm-6">
            <i class="fa fa-clock"></i>
            <div class="content">
              <h6>OPENING HOURS</h6>
              <p>Mon - Sat: 8.30am To 9.00pm</p>
            </div>
          </div>
           <div class="col-md-4 d-flex col-sm-6">
            <i class="fa fa-envelope-open"></i>
            <div class="content">
              <h6>SEND A MAIL</h6>
              <p><a href="mailto:example@example.com">example@example.com</a></p>
            </div>
          </div>
          <div class="col-md-4 d-none d-md-block">
            <a href="#appointment" class="topbar__btn">Get a Quote &nbsp;&nbsp;&nbsp; <i class="fa fa-long-arrow-alt-right"></i></a>
          </div>
        </div>
      </div>
      <!--End of Topbar section =======-->
      <!--Navbar section begins here ========-->
      <div class="navbar__wrapper">
        <div class="navbar__contents d-flex justify-content-between align-items-center">
          <div class="logo__brand">
            <router-link to="/" class="logo"><img src="../assets/images/logo.png" class="logo__img" alt=""></router-link>
          </div>
          <menu>
            <ul class="d-flex justify-content-between align-items-center">
              <li><router-link to="/">Home</router-link></li>
              <li><a href="#about">About Us</a></li>
              <li><a href="#services">Our Services</a></li>
              <li><a href="#appointment">Contact Us</a></li>
            </ul>
          </menu>
           <!-- <div @click="showNav()" class="navbar__toggler"> 
                    <div class="holder d-flex justify-content-between align-items-center">
                    <i class="fa fa-bars"></i>
                    <p class="pt-3 pl-2">Menu</p>
                    </div>
              </div> -->
        </div>
      </div>
      <!--End of Navbar section =====-->
      <!--Hero section begins here =======-->
      <div class="hero__section">
        <div class="row">
          <div class="col-12">
            <h1>We are qualified professionals that you can trust</h1>
            <router-link to="/contact" class="hero__btn">Explore More <i class="fa fa-long-arrow-alt-right"></i></router-link>
          </div>
        </div>
      </div>
    </div>
  </div>
  <Intro />
  <Features />
  <Services />
  <Appointment />
  <Gallery />
  <Testimonials />
  <Counter />
  <Footer />
  </div>
</template>

<script>
import Intro from '@/components/Intro.vue'
import Features from '@/components/Features.vue'
import Services from '@/components/Services.vue'
import Appointment from '@/components/Appointment.vue'
import Gallery from '@/components/Gallery.vue'
import Testimonials from '@/components/Testimonials.vue'
import Counter from '@/components/Counter.vue'
import Footer from '@/components/Footer.vue'
export default {
components:{
  Intro,
  Features,
  Services,
  Appointment,
  Gallery,
  Testimonials,
  Counter,
  Footer
}
}
</script>

<style lang="scss" scoped>
@import '../assets/styles/_colors';
.home{
  background: linear-gradient(rgba(0,0,0,.5), rgba(0,0,0,.5)), url('../assets/images/img1.jpg');
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
  height: 100vh;
  color: #fff;
  //Topbar styling
  .topbar{
    // background: red;
    padding-top: 3rem;
    margin-bottom: 1rem;
    .fa-clock, .fa-envelope-open{
      color: $secondary-color;
      font-size: 1.3rem;
      margin-right: 1rem;
    }
    .topbar__btn{
      background: $secondary-color;
      padding: 1rem 2rem;
      border-radius: 4px;
      color: #fff;
      font-size: .9rem;
      font-weight: bold;
      text-decoration: none;
      .fa-long-arrow-alt-right{
        margin-left: 1rem;
      }
    }
    .content{
      h6{
        font-weight: bold;
        font-size: .9rem;
      }
      p, a{
        font-size: .85rem;
        font-weight: 400;
        opacity: .95;
        color: #fff;
      }
    }
  }

  //Navbar styling
  .navbar__wrapper{
  background: #fff;
  padding: .4rem;
  .logo__img{
    max-width: 220px;
    height: auto;
  }
  .navbar__toggler{
            display: none;
            font-size: 1.2rem;
            padding-right: 1rem;
            color: $secondary-color !important;
        }
  menu{
    padding-top: 1rem;
    ul li a{
      color: $primary-color;
      margin: 0 3rem;
      display: block;
      font-weight: bolder;
      text-transform: uppercase;
      font-size: .9rem;
      text-decoration: none;
      &:hover{
        color: $secondary-color
      }
    }
  }
  }

  //Hero section styling
  .hero__section{
    padding-top: 10rem;
    h1{
      font-weight: bolder;
      padding-bottom: 3rem;
      text-shadow: 0.03em 0.03em 0.08em rgba(0,0,0,0.5);
      font-size: 4rem;
      text-transform: capitalize;
    }
    .hero__btn{
      background: $secondary-color;
      padding: 1.2rem 3rem;
      border-radius: 4px;
      color: #fff;
      font-size: .9rem;
      font-weight: bold;
      text-decoration: none;
      .fa-long-arrow-alt-right{
        margin-left: 1rem;
      }
    }
  }
}


//MEDIA QUERIES FOR THE NAVBAR SECTION
@media only screen and (max-width: 900px){
  .navbar__wrapper{
    padding-top: 4rem !important;
    background: transparent !important;
  }
  .navbar__toggler{
    display: block !important;
    font-size: 1.2rem;
    padding-right: 1rem;
    color: $secondary-color !important;
}
  menu{
        background-color: $primary-color;
        width: 85%;
        position: absolute;
        height: auto !important;
        z-index: 100;
        height: 100vh -50% !important;
        display: none;
        border-top: 3px solid $secondary-color;
        padding: 0 1rem !important;
        margin: 0 auto !important;
        transition: 0.5s !important;
        top: 100%;
        left: 7%;
        ul{
            flex-direction: column;
            li a{
                color: #fff !important;
                line-height: 4;
            }
        }
    }

    //HERO SECTION MEQIA QUERIES
    @media only screen and (max-width: 600px){
      .home{
      height: 80vh !important;
    }
    .hero__section{
      padding-top: 8rem !important;
      text-align: center;
      h1{
        font-size: 2.5rem !important;
      }
    }
    }
}
</style>
