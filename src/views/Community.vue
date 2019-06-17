<template>
    <div>
        <PHeader />
        <CommunityHeader/>
        <div class="mt-10 row ml-mr" id="">
            <!-- Grid column -->
                <div class="col-md-3 mr-10">
                    <div class="">
                        <img style="width:100%" class="img-fluid" src="../assets/images/left.png" alt="Card image cap">
                    </div>
                </div>
                <div class="col-md-3 mr-10">
                    <div class="">
                         <img style="width:100%" class="img-fluid mb-6" src="../assets/images/middle-top.png" alt="Card image cap">
                        <img style="width:100%" class="img-fluid" src="../assets/images/middle-bottom.png" alt="Card image cap">
                    </div>
                   
                </div>
                <div class="col-md-5 mr-10 ">
                     <div class="">
                        <img  class="img-fluid mb-6" src="../assets/images/right-top.png" alt="Card image cap"
                        style="object-fit:contain;width:100%">
                        <img class="img-fluid" src="../assets/images/right-bottom.png" alt="Card image cap"
                        style="object-fit:contain;width:100%">
                    </div>
                </div>
        </div>
        <div id="mobile-gallery" class="">
            <div class="col-6">
                 <div class="mg-b pics all 2 animation" style="">
                    <img class="img-fluid" style="height:271px;width:100%" src="../assets/images/left.png" alt="Card image cap">
                </div>
            </div>
            <div class="col-6">
                <div class="mg-b pics all 1 animation" style="">
                    <img class="img-fluid" style="height:142px;width:100%" src="../assets/images/middle-top.png" alt="Card image cap">
                </div>
                <div class="mg-b pics all 1 animation" style="">
                    <img class="img-fluid" src="../assets/images/middle-bottom.png" alt="Card image cap"
                        style="height: 118px;width: 100%;">
                </div>
            </div>
        </div>
        <section class="xs-section-padding">
            <div class="container">
                <div class="row">
                    <div class="col-lg-10 mx-auto">
                        <div class="agency-section-title text-center section-title-style2">
                            <h2 class="main-title join-com">Why Join the Community?</h2>
                        </div>
                    </div>
                </div><!-- .row end -->
                  <div id="carouselIndicators" class="carousel slide" data-ride="carousel">
                     
                    <ol class="carousel-indicators">
                         
                        <li data-target="#carouselIndicators" data-slide-to="0" class="active"></li>
                        <li data-target="#carouselIndicators" data-slide-to="1"></li>
                        <li data-target="#carouselIndicators" data-slide-to="2"></li>
                        <li data-target="#carouselIndicators" data-slide-to="3"></li>
                         
                         
                    </ol>
                    <div class="carousel-inner">
                        <div class="carousel-item active">
                            <div class="row">
                                    <div class="col-md-4">
                                        <p class="big-p">
                                            Meet Great Minds
                                        </p>
                                        <p class="small-p">
                                            Lorem ipsum dolor sit amet, consectetur adipiscing elit
                                        </p>
                                    </div>
                                    <div class="col-md-8">
                                        <img src="../assets/images/sunmisola-olorunnisola-43913798-184315472451375-8597409187659397510-n.png"
                                            alt="">
                                    </div>
                                </div>
                        </div>
                        <div class="carousel-item">
                            <div class="row">
                                    <div class="col-md-4">
                                        <p class="big-p">
                                            Show case
                                        </p>
                                        <p class="small-p">
                                            Lorem ipsum dolor sit amet, consectetur adipiscing elit
                                        </p>
                                    </div>
                                    <div class="col-md-8">
                                        <img src="../assets/images/grid-image.png"
                                            alt="">
                                    </div>
                                </div>
                        </div>
                        <div class="carousel-item">
                             <div class="row">
                                    <div class="col-md-4">
                                        <p class="big-p">
                                            Get Support
                                        </p>
                                        <p class="small-p">
                                            Lorem ipsum dolor sit amet, consectetur adipiscing elit
                                        </p>
                                    </div>
                                    <div class="col-md-8">
                                        <img src="../assets/images/support-image-copy.png"
                                            alt="">
                                    </div>
                                </div>
                        </div>
                         <div class="carousel-item">
                             <div class="row">
                                    <div class="col-md-4">
                                        <p class="big-p">
                                            Learn
                                        </p>
                                        <p class="small-p">
                                            Lorem ipsum dolor sit amet, consectetur adipiscing elit
                                        </p>
                                    </div>
                                    <div class="col-md-8">
                                        <img src="../assets/images/learn-image-copy.png"
                                            alt="">
                                    </div>
                                </div>
                        </div>
                    </div>
                
            </div>
                 
                <div class="agency-section-title text-center section-title-style2">
                  <router-link class="" to="/community/join">
                    <button class="btn btn-p btn-rounded btn-peexoo">Join now</button>
                  </router-link>
                    
                </div>
            </div><!-- .container END -->
        </section><!-- end business info section -->
        <section class="">
            <div class="container">
                <div class="row">
                    <div class="col-lg-10 mx-auto">
                        <div class="agency-section-title text-center section-title-style2">
                            <h2 class="main-title main-title-t" style="color:#ffb503">These Legends are Community
                                Members</h2>
                        </div>
                    </div>
                </div><!-- .row end -->
                <div class="row">
                    <div class="row">
                        <div class="col-md-2 col-6 legend-img">
                            <img src="../assets/images/kelechi.png" alt="">
                            <h5 class="text-center">Kelechi Amadi Obi</h5>
                        </div>
                        <div class="col-md-2 col-6 legend-img">
                            <img src="../assets/images/afroshots.png" alt="">
                            <h5 class="text-center">Afroshots</h5>
                        </div>
                        <div class="col-md-2 col-6 legend-img">
                            <img src="../assets/images/kelechi.png" alt="">
                            <h5 class="text-center">Kelechi Amadi Obi</h5>
                        </div>
                        <div class="col-md-2 col-6 legend-img">
                            <img src="../assets/images/afroshots.png" alt="">
                            <h5 class="text-center">Afroshots</h5>
                        </div>
                        <div class="col-md-2 col-6 legend-img">
                            <img src="../assets/images/kelechi.png" alt="">
                            <h5 class="text-center">Kelechi Amadi Obi</h5>
                        </div>
                        <div class="col-md-2 col-6 legend-img">
                            <img src="../assets/images/afroshots.png" alt="">
                            <h5 class="text-center">Afroshots</h5>
                        </div>
                    </div>
                </div>
            </div><!-- .container END -->
        </section><!-- end business info section -->
        <section class="how-works">
            <div class="container">
                <div class="row">
                    <div class="col-lg-10 mx-auto">
                        <div class="agency-section-title text-center section-title-style2">
                            <h2 class="main-title main-title-t" style="color:#ffb503">How it works</h2>
                        </div>
                    </div>
                </div><!-- .row end -->
                <div class="row">
                    <div class="col-md-8 offset-md-2 desktop">
                        <div class="row">
                            <div class="col-md-4 ">
                                <img class="" src="../assets/images/login.svg" alt="">
                                <h5 class="text-center how-text">Sign up</h5>
                            </div>
                            <div class="col-md-4 ">
                                <img class=""
                                    src="../assets/images/verified.svg" alt="">
                                <h5 class="text-center how-text">Get Vetted</h5>
                            </div>
                            <div class="col-md-4">
                                <img class="" src="../assets/images/community.svg" alt="">
                                <h5 class="text-center how-text">Attend meetups</h5>
                            </div>
                        </div>

                    </div>
                    <div class="row mobile-steps">
                        
                        <div class="col-4 ">
                            <img class="" src="../assets/images/login.svg" alt="">
                            <h5 class="text-center how-text">Sign up</h5>
                        </div>
                        <div class="col-4 ">
                            <img class=""
                                    src="../assets/images/verified.svg" alt="">
                            <h5 class="text-center how-text">Get Vetted</h5>
                        </div>
                        <div class="col-4">
                            <img class="" src="../assets/images/community.svg" alt="">
                            <h5 class="text-center how-text">Attend meetups</h5>
                        </div>
                    </div>
                </div>
                <div class="agency-section-title text-center section-title-style2">
                     <router-link class="" to="/community/join">
                        <button class="btn btn-p btn-rounded btn-peexoo">Join now</button>
                  </router-link>
                </div>
            </div><!-- .container END -->
        </section>
        <PhotoTestimony />
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
                                <img style="width:40%" src="../assets/images/ww_app-store.png"
                                    alt="download from app store">
                            </span>
                            <span>
                                <img style="width:45%" src="../assets/images/google-play.png"
                                    alt="download from google store">
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
    import Footer from '../components/Footer'
    import Menu from '../components/Menu'
    import PhotoTestimony from '../components/Photo-Testimony'
    import CommunityHeader from '../components/community-header'
  

    export default {
        name: "community",
        components: {
            PHeader,
            Footer,
            Menu,
            PhotoTestimony,
            CommunityHeader
        },
        methods: {
             
        }

    }
</script>
<style scoped>
    .col-md-3, .col-md-5, .row{
        padding-right: 0px !important;
        padding-left: 0px !important
    }
    .col-md-3{
        flex: 0 0 28% !important;
        max-width: 28% !important;
    }
    .col-md-5{
        flex: 0 0 39.92% !important;
        max-width: 39.92% !important;
    }
    .ml-mr{
        margin-left: 10px;
        
    }
    .how-works {
        margin-top: 100px
    }

    .how-text {
        font-size: 18px;
        color: #4d4d4d;
        margin-top: -25px;
    }

    .join-com {
        margin-bottom: 70px !important
    }

    .legend-img h5 {
        font-size: 16px;
        margin-top: 10px;
        color: #646464;
    }
    .col-md-2 {
        padding-right: 10px !important;
        padding-left: 10px !important;
    }

    .agency-section-title .main-title {
        font-size: 64px !important;
    }

    .agency-section-title .main-title-t {
        font-size: 48px !important;
    }

   

    .big-p {
        padding-bottom: 25px;
        font-family: 'Montserrat';
        font-size: 85px;
        font-weight: bold;
        font-style: normal;
        font-stretch: normal;
        line-height: normal;
        letter-spacing: normal;
        color: #4d4d4d;
    }

    .small-p {
        font-size: 43px;
        font-weight: normal;
        font-style: normal;
        font-stretch: normal;
        line-height: normal;
        letter-spacing: normal;
        color: #4d4d4d;
    }

    .mt-10 {
        margin-top: 10px !important
    }

    .mg-b {
        margin-bottom: 11px !important;
    }
    .mb-6 {
        margin-bottom: 6px !important;
    }
    .mr-10{
        margin-right: 12px !important
    }
     

    .gallery {
        -webkit-column-count: 3;
        -moz-column-count: 3;
        column-count: 3;
        -webkit-column-width: 33%;
        -moz-column-width: 33%;
        column-width: 33%;
    }

    .gallery .pics {
        -webkit-transition: all 350ms ease;
        transition: all 350ms ease;
    }

    .gallery .animation {
        -webkit-transform: scale(1);
        -ms-transform: scale(1);
        transform: scale(1);
    }
    #mobile-gallery{
        display: none
    }
    .mobile-steps{
        display: none
    }
    @media (max-width: 480px) {
        .how-works{
            margin-top:0 !important
        }
        .how-text{
            margin-top: 0px !important;
        }
        .desktop{
            display: none
        }
        .mobile-steps{
            display: flex
        }
        .legend-img img{
            padding-left: 7px;
            padding-right: 7px;
        }
        .row{
            margin-right: 0 !important ;
            margin-left: 0 !important
        }
        #gallery{
            display: none
        }
        #mobile-gallery{
        display: flex;
        margin-top: 10px;
        margin-right: 5px !important;
        margin-left: 5px !important;
        }
        .agency-section-title .main-title{
            font-size: 36px !important;
            margin-top: 71px;
            font-weight:700;
        }
        .agency-section-title .main-title .main-title-t{
            font-size: 28px !important;
            font-weight:700;
        }
        .col-6{
            padding-right: 5px !important;
            padding-left: 5px !important;
        }
        .gallery {
            -webkit-column-count: 1;
            -moz-column-count: 1;
            column-count: 1;
            -webkit-column-width: 100%;
            -moz-column-width: 100%;
            column-width: 100%;
        }
    }

    @media (max-width: 400px) {
        .btn.filter {
            padding-left: 1.1rem;
            padding-right: 1.1rem;
        }
    }
</style>