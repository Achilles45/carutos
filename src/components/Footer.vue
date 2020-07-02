<template>
  <footer class="footer">
     <div class="top__footer">
          <div class="container">
          <div class="row">
              <div class="col-md-6">
                  <img src="../assets/images/logo.png" class="footer__logo" alt="">
                  <h6>A major key, never panic. Don’t panic, when it gets crazy and rough, don’t panic, stay calm. They will try to close the door on you, just open it. Another one.</h6>
              </div>
              <div class="col-md-1"></div>
               <div class="col-md-4">
                  <h5>Contact Info</h5>
                  <h6>Address: 1379 Shoreline Parkway, Mountain View, CA 94043, United States.</h6>
                  <h6>Email: <a href="mailto:example@mail.com">Example@mail.com</a></h6>
              </div>
              <!-- <div class="col-md-4">
                  <h5>Company Links</h5>
                  <ul>
                      <li><router-link to="/">Home</router-link></li>
                      <li><router-link to="/">Home</router-link></li>
                      <li><router-link to="/">Home</router-link></li>
                      <li><router-link to="/">Home</router-link></li>
                      <li><router-link to="/">Home</router-link></li>
                  </ul>
              </div> -->
          </div>
      </div>
     </div><br>
     <div class="footer__bottom">
         <div class="container">
             <div class="row text-center">
                 <p>Copyright &copy; 2020. All rights reserved.</p>
             </div>
         </div>
     </div>
  </footer>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import '../assets/styles/_colors';
footer{
    padding-top: 5rem;
    .footer__logo{
        max-width: 250px;
        height: auto;
        padding-bottom: 2rem;
    }
    h6{
        line-height: 1.6;
         color: #627081;
    }
    h5{
        font-weight: bold;
        color: $primary-color;
        padding-bottom: 2rem;
        opacity: .8;
    }
    a{
        color: #627081;
        text-decoration: none;
        font-weight: 400;
    }
    .footer__bottom{
        background: $primary-color;
        color: #fff !important;
        padding: 1rem;
        text-align: center;
    }
}
</style>
