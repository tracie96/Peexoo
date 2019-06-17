<template>
  <div id="app" class="page">
    <PHeader />
    <section class="banner-area-wraper">
      <div class="banner-slider-area">
       <Appslider/>
      </div>
      <p class="p-slider">
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
              <h2 class="main-title">Beyond Photography</h2>
              <p>
                Quick and easy way to find World class photographers to capture and preserve your beautiful
                memories combining human creativity and artificial intelligence.
              </p>

              <button class="btn btn-p btn-rounded btn-peexoo">Explore Photos</button>
            </div>
          </div>
        </div><!-- .row end -->

      </div><!-- .container END -->
    </section><!-- end business info section -->
    <Booking />
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
  import PHeader from '../components/PHeader'
  import Booking from '../components/Booking'
  import Testimony from '../components/Testimony'
  import Footer from '../components/Footer'
  import Menu from '../components/Menu'
  import Appslider from '../components/App-slider'
  
 
  export default {
    name: "home",
    components: {
      PHeader,
      Booking,
      Testimony,
      Footer,
      Menu,
      Appslider
      
       
    }
   
}

</script>
<style >
   
        .form-wrapper-outer {
            padding: 40px;
            border-radius: 8px;
            margin: auto;
            width: 460px;
            border: 1px solid #DADCE0;
            margin-top: 7%;
        }
    
        .form-wrapper-outer .form-logo {
            margin: 0px auto 15px;
            width: 100px;
        }
    
        .form-wrapper-outer .form-logo img {
            width: 100%;
        }
    
        .form-greeting {
            text-align: center;
            font-size: 25px;
            margin-bottom: 15px;
        }
    
        .form-button {
            text-align: right;
        }
    
        .field-wrapper {
            position: relative;
            margin-bottom: 15px;
        }
    
        .field-wrapper input {
            border: 1px solid #979797;
            padding: 15px;
            border-radius: 5px;
            width: 100%;
        }
    
        .field-wrapper .field-placeholder {
            font-size: 16px;
            position: absolute;
            /* background: #fff; */
            bottom: 17px;
            -webkit-box-sizing: border-box;
            box-sizing: border-box;
            color: #80868b;
            left: 8px;
            padding: 0 8px;
            -webkit-transition: transform 150ms cubic-bezier(0.4, 0, 0.2, 1), opacity 150ms cubic-bezier(0.4, 0, 0.2, 1);
            transition: transform 150ms cubic-bezier(0.4, 0, 0.2, 1), opacity 150ms cubic-bezier(0.4, 0, 0.2, 1);
            z-index: 1;
    
            text-align: left;
            width: 100%;
        }
    
        .field-wrapper .field-placeholder span {
            background: #ffffff;
            padding: 0px 0px;
            font-size: 13px;
        }
    
        .field-wrapper input:not([disabled]):focus~.field-placeholder {
            color: #b58000;
        }
    
        .field-wrapper input:not([disabled]):focus~.field-placeholder,
        .field-wrapper.hasValue input:not([disabled])~.field-placeholder {
            -webkit-transform: scale(.75) translateY(-39px) translateX(-60px);
            transform: scale(.75) translateY(-39px) translateX(-60px);
    
        }
        
    </style>