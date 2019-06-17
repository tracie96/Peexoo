<template>
    <div>
        <PHeader/>
        <CommunityHeader />
        <section class="xs-section-padding mb-15">
            <div class="container">
                <div class="row">
                    <div class="col-md-6 col-12">
                        <form>
                            <p class="h6 mb-4">Kindly fill out this form to join the community</p>
                             
                            <mdb-input type="text"  label="Enter your first name" outline />
                           
                            <mdb-input  type="text"  label="Enter your last name" outline />
                        
                            <mdb-input type="email"  label="Enter your email" outline />
                           
                            <mdb-input  type="number"  label="Enter your phone number" outline />

                            <select class="browser-default custom-select">
                                <option selected>How did you hear about the community?</option>
                                <option value="1">One</option>
                                <option value="2">Two</option>
                                <option value="3">Three</option>
                            </select>

                            <mdb-input type="textarea" placeholder='Any other comment?'  outline :rows="3" />

                            <div class="text-center mt-4">
                                <button style="width: 100%;color:#fff" class="btn btn-p btn-rounded btn-peexoo">JOIN THE COMMUNITY</button>
                            </div>
                        </form>
                    </div>
                    <div class="col-md-6 desktop-only">
                        <img src="../assets/images/sunmisola-olorunnisola-43913798-184315472451375-8597409187659397510-n.png"
                        alt="">
                    </div>
                </div><!-- .row end -->

            </div><!-- .container END -->
        </section><!-- end business info section -->
         <Footer />
        <Menu />
    </div>
</template>
<script>
    import PHeader from '../components/PHeader'
    import Footer from '../components/Footer'
    import Menu from '../components/Menu'
    import CommunityHeader from '../components/community-header'
    import { mdbInput } from "mdbvue";
    export default {
        name: "join-community",
        components: {
            PHeader,
            Footer,
            Menu,
            CommunityHeader,
            mdbInput
        }

    }
</script>
<style scoped>

@media screen and (max-width: 480px) {
    .xs-section-padding{
        padding-top:50px!important;
    }
    .desktop-only{
        display:none
    }
    .mb-15{
        margin-bottom: 30px !important
    }
}
</style>
