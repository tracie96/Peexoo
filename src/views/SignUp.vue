<template>
    <div>
        <PHeader />
        <form class="form-m" id="registerform" @submit.prevent="submit">
            <div id="top-d">
                <p class="sign">
                    Sign Up
                </p>

            </div>
            <mdb-input type="text"  label="Enter your first name" outline v-model="registerForm.first_name"/>
                           
            <mdb-input  type="text"  label="Enter your last name" outline v-model="registerForm.last_name" />
                        
            <mdb-input type="email"  label="Enter your email" outline v-model="registerForm.email" />
                                            
            <mdb-input type="password"  label="Enter your password" outline v-model="registerForm.password" />
             
            <div class="row">
                <div class="col-md-12">
                    <div class="checkbox">
                        <label class="check-label">
                            <input class="keep-me" type="checkbox"> I have agreed to the <router-link class="log"
                                to="/terms">terms and conditions</router-link> of peexo.ai
                        </label>
                    </div>
                </div>

            </div>
            <div class="row text-center" style="margin-top:20px">

                <div class="col-md-12">
                    <button id="btn-p" class="btn btn-rounded btn-peexoo text-white">SIGN
                        UP</button>
                </div>

            </div>
            <div class="login-flex-parent" style="margin-top:40px">
                <div class="flex-child-edge"></div>
                <div class="login-flex-child-text">or sign up with</div>
                <div class="flex-child-edge"></div>
            </div>
            <div class="row text-center" style="margin-top:20px">

                <div class="col-md-6 offset-md-3">
                    <a href="#"><i class="fa fa-facebook"></i></a>
                    <a href="#"><i class="fa fa-google"></i></a>
                </div>

            </div>
            <p class="text-center not-member">
                Already a member? <router-link class="log" to="/login">Sign in</router-link>
            </p>
        </form>
    </div>
</template>
<script>
    import PHeader from '../components/PHeader'
    import { mdbInput } from 'mdbvue';
    export default {
        name: "home",
        components: {
            PHeader,
            mdbInput
        },
         data() {
            return {
                registerForm: {
                    email: '',
                    password: '',
                    // password_confirmation: '',
                    first_name: '',
                    last_name: '',
                     
                }
            }
        },
        methods: {
            // submit(e) {
            //     axios.post('/api/auth/register', this.registerForm).then(response => {
            //         toastr['success'](response.data.message);
            //         //this.$router.push('/user');
            //     }).catch(error => {
            //         toastr['error'](error.response.data.message);
            //     });
            // },
            
        }
    }
  
</script>

<style scoped>
    .not-member {
        font-size: 12px;
        font-weight: normal;
        font-style: normal;
        font-stretch: normal;
        line-height: normal;
        letter-spacing: normal;
        text-align: center;
        color: #414141;
        margin-top: 20px
    }

    .keep-me {
        font-size: 16px;
    }

    #btn-p {
        width: 100%;
    }

    #top-d {
        margin-bottom: 20px
    }

    .forget {
        font-family: 'Montserrat';
        font-size: 12px;
        font-weight: normal;
        font-style: normal;
        font-stretch: normal;
        line-height: normal;
        letter-spacing: normal;
        color: #b58000;
    }

    .sign {
        font-family: Lora !important;
        font-size: 24px;
        font-weight: bold;
        font-style: normal;
        font-stretch: normal;
        line-height: normal;
        letter-spacing: normal;
        color: #414141;
        margin-bottom: 1px;
    }

    .close-btn {
        position: absolute;
        right: -1rem;
        top: -1rem;
        z-index: 1000;
        background: #d8d8d8;
        border-radius: 50%;
        padding: 6px;
        color: #4f4f4f;
        font-weight: normal;
    }

    .log {
        color: #b58000 !important;
        cursor: pointer !important;
    }

    .li-m {
        width: 50%;
        padding-top: 15px;
        text-align: center;
        background: #fefbf3;
    }

    .li-m a {
        padding: 18px 109px 22px 77px;

    }

    a.active {
        background: #ffb503
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

    .login-flex-parent {
        display: flex;
        width: 100%;
        height: 0px;
        align-items: center;
    }

    .login-flex-child-text {
        flex-basis: auto;
        flex-grow: 0;
        margin: 0px 25px 0px 25px;
        text-align: center;
        font-size: 12px;
        font-weight: 400;
        color: #4d4d4d;
    }

    .width-15 {
        width: 15% !important;
    }

    .width-85 {
        width: 85% !important;
    }

    .flex-parent {
        display: flex;
        width: 300px;
        height: 20px;
        align-items: center;
        margin-bottom: 20px;

    }

    .flex-child-edge {
        flex-grow: 2;
        height: 1px;
        background-color: #000;
        border: 1px #979797 solid;
    }

    .flex-child-text {
        flex-basis: auto;
        flex-grow: 0;
        margin: 0px 5px 0px 5px;
        text-align: center;
        font-size: 11px;
    }

   .fa-facebook {
        background: #3b5998;
        padding: 13px 10px 1px 12px;
        border-radius: 50%;
        color: #fff;
        height: 40px;
        width: 40px;
        margin-right: 10px;
    }

    .fa-google {
        background: #db4a39;
        padding: 13px 9px 0px 11px;
        border-radius: 50%;
        color: #fff;
        height: 40px;
        width: 40px;

    }

    .terms {
        color: #be7e00 !important;
        font-family: 'Montserrat';
    }
</style>