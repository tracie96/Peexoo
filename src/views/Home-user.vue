<template>
    <div>
    <Header />
    <section class="banner-area-wraper">
      <div class="banner-slider-area">
       <Appslider/>
      </div>
      <p class="text-left ml-5">
        <span id="title-banner">
          KELECHI AMADI OBI 
        </span>
      </p>
    </section><!-- end agency banner section -->
    <section class="xs-section-padding">
        <div class="container">
            <div class="row">
                <div class="col-lg-10 mx-auto">
                    <div class="agency-section-title text-center section-title-style2">
                        <h2 class="main-title">Seamless Photography Business</h2>
                        <p>
                            We help photographers find, retain and grow their customer base and brand.
                        </p>

                        <button class="btn btn-p btn-rounded btn-peexoo">Join the Community</button>
                    </div>
                </div>
            </div><!-- .row end -->

        </div><!-- .container END -->
    </section><!-- end business info section -->
    <!-- business info section -->
    <section class="">
        <div class="container">
            <div class="row">
                <div class="col-lg-10 mx-auto">
                    <div class="agency-section-title text-center section-title-style2">
                        <h2 class="main-title  users-say" style="color:#ffb503">How it works</h2>

                    </div>
                </div>
            </div><!-- .row end -->
            <div class="row">
                <div class="col-md-8 offset-md-2">
                    <div class="row">
                        <div class="col-md-6 col-lg-3 col-6">
                            <div class="circle circle-black text-center">
                                <div>
                                    Register
                                </div>
                            </div>
                        </div>
                        <div class="col-md-6 col-lg-3 col-6">
                            <div class="circle circle-black text-center">
                                <div>
                                    Accept
                                    Booking
                                    Request
                                </div>
                            </div>
                        </div>
                        <div class="col-md-6 col-lg-3 col-6">
                            <div class="circle circle-black text-center">
                                <div>
                                    Shoot
                                </div>
                            </div>
                        </div>
                        <div class="col-md-6 col-lg-3 col-6">
                            <div class="circle circle-black text-center">
                                <div>
                                    Get Paid
                                </div>
                            </div>
                        </div>
                    </div><!-- .row END -->
                </div>
            </div>
        </div><!-- .container END -->
    </section><!-- end business info section -->
 <Testimony />
       
    <section class="xs-section-padding" style="padding-bottom:80px">
      <div class="container">
        <div class="row pexo-bg">
          <div class="col-md-6 pexo-pad">
            <p>
              DON’T MISS OUT!
              DOWNLOAD OUR MOBILE APP
              FOR A FULL MOBILE
              EXPERIENCE
            </p>
            <div class="pad-top-30">
              <span>
                <img style="width:40%" src="../assets/images/ww_app-store.png" alt="download from app store">
              </span>
              <span>
                <img style="width:45%" src="../assets/images/google-play.png" alt="download from google store">
              </span>
            </div>
          </div>
          <div class="col-md-6 pexo-pad">
            <img src="../assets/images/app-screen-mockup.png" alt="">
          </div>
        </div>
      </div>
    </section>
    <Footer />
  
    <Menu />
    </div>
</template>

<script>
  import Header from '../components/Header'
  import Testimony from '../components/Testimony'
  import Footer from '../components/Footer'
  import Menu from '../components/Menu'
  import Appslider from '../components/App-slider'
 
  export default {
    name: "home-user",
    components: {
      Header,
      Testimony,
      Footer,
      Menu,
      Appslider,  
    }
}
</script>

