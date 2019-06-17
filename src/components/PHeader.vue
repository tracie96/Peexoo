<template>
    <div>
        <login-register :show="showloginModal" @close="showloginModal = false"></login-register>
         <header class="xs-header header-transparent header-style2 desktop">
            <div class=" ">
                <nav class="xs-menus clearfix fixed-head">
                    <div class="nav-header">
                        <a class="nav-brand" href="">
                            <img src="../assets/images/asset-7.png" alt="">
                        </a>
                        <div class="nav-toggle"></div>
                    </div>
                    <div class="nav-menus-wrapper align-to-right">
                        <!-- menu list -->
                        <ul class="nav-menu">
                            <li>
                                <router-link to="/photographers">I am a Photographer</router-link>  
                            </li>
                            <li><a href="">Explore Photos</a></li>
                            <li>
                                <router-link to="/photographers/search">Find a Photographer</router-link>
                            </li>
                            <li>
                                <a href="">Find my photos</a>
                            </li>
                            <li><a class="log_x" @click="showloginModal = true"  style="color:rgb(255, 181, 3)">Login or
                                    Register</a></li>
                        </ul>

                    </div>
                </nav>
            </div><!-- .container END -->
        </header><!-- End header section -->

         
            <!--Navbar-->
            <mdb-navbar  class="mobile-head" animated animation="1">
                <!-- Navbar brand -->
                <mdb-navbar-brand class="left">
                    <router-link class="" to="/">
                        <img src="../assets/images/asset-7.png" alt="">
                    </router-link>
                    
                </mdb-navbar-brand>
                <mdb-navbar-toggler>
                    <mdb-navbar-nav right>
                        <mdb-nav-item waves-fixed>
                            <router-link class="" to="/photographers">I am a Photographer</router-link>
                        </mdb-nav-item>
                        <mdb-nav-item href="#" waves-fixed>Explore Photos</mdb-nav-item>
                       <router-link class="" to="/photographers/search">
                            <mdb-nav-item waves-fixed>Find a Photographer</mdb-nav-item>
                        </router-link>
                        <mdb-nav-item href="#" waves-fixed>Find my photos</mdb-nav-item>
                        <router-link class="log" to="/login">
                            <mdb-nav-item waves-fixed>Login</mdb-nav-item>
                        </router-link>
                        <router-link class="log" to="/signup">
                            <mdb-nav-item waves-fixed>Register</mdb-nav-item>
                        </router-link>
                         
                    </mdb-navbar-nav>
                </mdb-navbar-toggler>
            </mdb-navbar>
         
    </div>
</template>
<script>
    
    import LoginRegister from './login-register'
    import { mdbNavbar, mdbNavItem, mdbNavbarNav, mdbNavbarToggler,mdbNavbarBrand } from 'mdbvue';
    export default {
        props: ['show'],
        data: function () {
            return {
                showloginModal:false,
                loading: true
            }
        },
        components: {
            LoginRegister,
            mdbNavbar,
            mdbNavItem,
            mdbNavbarNav,
            mdbNavbarToggler,
            mdbNavbarBrand
        },
        // updated: function () {
        //     document.addEventListener("keydown", (e) => {
        //         if (this.showloginModal && e.keyCode == 27) {
        //             this.close();
        //         }
        //     });
            
        // },
        methods:{
            // close: function () {
            //     this.showloginModal = false;
            // },
        }

    }
</script>


<style scoped>
    .log {
        color: #b58000 !important;
        cursor: pointer !important;
    }
    .text-white {
        color: #fff !important
    }

    input:internal-autofill-selected {
        background: #fff !important
    }

    button {
        box-shadow: none !important;
        height: 42px !important;
        line-height: 42px !important;
    }

    .pass-label {
        color: #b58000 !important;
        font-family: 'Montserrat';
        font-size: 12px;
        float: right;
    }

    .check-label {
        font-family: 'Montserrat';
        font-size: 12px
    }
    .width-15 {
        width: 15% !important;
    }

    .width-85 {
        width: 85% !important;
    }    
</style>