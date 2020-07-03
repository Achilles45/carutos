<template>
  <div class="appointment" id="appointment">
          <div class="container">
              <div class="row">
              <!-- <div class="col-md-6">
                 <div class="first">
                     <div class="text text-center">
                     <h2>Make Appointment</h2>
                     <p>A customer support agent will contact you to inform you about progress on your recommendation. </p>
                 </div>
                 <form action="">
                     <div class="row">
                         <div class="col-md-6">
                             <div class="form-group">
                                 <input type="text" class="form-control" placeholder="Name">
                             </div>
                         </div>
                         <div class="col-md-6">
                             <div class="form-group">
                                 <input type="tel" class="form-control" placeholder="Email">
                             </div>
                         </div>
                     </div>
                     <div class="row">
                         <div class="col-md-6">
                             <div class="form-group">
                                 <input type="text" class="form-control" placeholder="Phone">
                             </div>
                         </div>
                         <div class="col-md-6">
                             <div class="form-group">
                                <select class="form-control">
                                    <option value="" disabled selected>Select Service</option>
                                    <option value="Car registration">Car Registration</option>
                                    <option value="Car registration">Car Clearance</option>
                                    <option value="Car registration">Car Maintenance</option>
                                </select>
                             </div>
                         </div>
                     </div>
                     <textarea class="form-control" cols="30" rows="10" placeholder="Let's us know what you need"></textarea>
                     <div class="button__holder pt-5 pb-5 text-center">
                         <button type="submit" class="form__btn">Send Message</button>
                     </div>
                 </form>
                 </div>
              </div> -->
              <div class="col-md-2"></div>
              <div class="col-md-8 text-center right">
                  <div class="container">
                      <h2>Premium car service matched with great workmanship.</h2><br>
                      <div class="number">
                          <h1 class="num1">26</h1><br>
                          <h5>years of experience</h5><br>
                          <h6><i class="fa fa-envelope-open"></i><a href="mailto:info@carutos.com">info@carutos.com</a></h6>
                      </div>
                  </div>
              </div>
              <div class="col-md-2"></div>
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
.appointment{
    background: linear-gradient(rgba(4,9,30,.5),rgba(4,9,30,.5)), url('../assets/images/img4.jpg');
    background-size: cover;
    background-position: center;
    color: #fff;
    .first{
        background: #fff;
        padding: 0 3rem;
        .text{
            padding-top: 4rem;
            padding-right: 2rem;
            padding-bottom: 2rem;
            h2{
                color: $primary-color;
                font-weight: bold;
                font-size: 3.2rem;
                line-height: 1.3;
                text-transform: capitalize;
                padding-bottom: 1rem;
            }
            p{
                font-weight: 400;
                padding-bottom: .5rem;
                font-size: .9rem;
                color: #627081;
            }
        }
        form{
            input, select{
                background: #F6F6F6;
                border-radius: 0px;
                box-shadow: none;
                height: 3.2rem;
                border: #F6F6F6;
                font-size: .9rem;
            }
            textarea{
                height: 10rem;
                background: #F6F6F6;
                box-shadow: none;
                border: #F6F6F6;
                font-size: .9rem;
                border-radius: 0px;
                padding: 1rem ;
            }
            .form__btn{
                background: $secondary-color;
                text-decoration: none;
                border: none;
                padding: 1rem 2rem;
                color: #fff;
                font-size: .8rem;
                font-weight: bold;
            }
        }
    }
    .right{
        padding: 8rem 1rem;
        h2{
            text-transform: capitalize;
            font-weight: 900;
            line-height: 1.5;
            font-size: 2.5rem;
        }
        .num1{
            color: $secondary-color;
            font-size: 8rem;
            font-weight: bold;
        }
        h5{
            font-weight: bold;
        }
        .fa-envelope-open{
            color: $secondary-color;
            margin-right: 1rem;
            font-size: 1.5rem;
        }
        h6{
            color: #fff;
            font-weight: bold;
        }
        a{
            color: #fff;
        }
    }
}

//Media Queries

</style>