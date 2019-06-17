<template>
<div>
    <modal :show="showConfirmPasswordModal" @close="showConfirmPasswordModal = false"></modal>
      <transition name="modal">
        <div class="modal-mask" v-show="show">
            <div class="modal-container">
                <div class="modal-dialog" role="document">
                    <div class="modal-content">
                        <i class="fa fa-times close-btn" @click="close"></i>
                        <div class="row"  >
                            <div class="col-md-12">
                                <div>
                                    <!-- Nav tabs -->
                                    <ul class="nav nav-tabs nav-justified" role="tablist">
                                        <li role="presentation" class="active li-m"><a href="#signin"
                                                aria-controls="signin" role="tab" data-toggle="tab" class="active">Sign
                                                in</a>
                                        </li>
                                        <li role="presentation" class="li-m"><a href="#signup" aria-controls="signup"
                                                role="tab" data-toggle="tab">Sign
                                                Up</a></li>
                                    </ul>
                                    <!-- Tab panes -->
                                    <div class="tab-content">
                                        <div role="tabpanel" class="tab-pane active" id="signin">
                                            <form class="form-m" id="loginform" @submit.prevent="login">

                                                <mdb-input type="email" name="email" label="Enter your email" outline />

                                                <mdb-input type="password" name="password" label="Enter your password"
                                                    outline />
                                                <div class="row">
                                                    <div class="col-md-6">
                                                        <div class="checkbox">
                                                            <label class="check-label">
                                                                <input type="checkbox"> keep me Logged in
                                                            </label>
                                                        </div>
                                                    </div>
                                                    <div class="col-md-6">
                                                        <a class="pass-label" for="">Forgot your password?</a>
                                                    </div>
                                                </div>
                                                <div class="row text-center" style="margin-top:20px">

                                                    <div class="col-md-6 offset-md-3">
                                                        <button class="btn btn-rounded btn-peexoo text-white">SIGN
                                                            IN</button>
                                                    </div>

                                                </div>
                                                <div class="login-flex-parent" style="margin-top:40px">
                                                    <div class="flex-child-edge"></div>
                                                    <div class="login-flex-child-text">or sign in with</div>
                                                    <div class="flex-child-edge"></div>
                                                </div>
                                                <div class="row text-center" style="margin-top:20px">

                                                    <div class="col-md-6 offset-md-3">
                                                        <a href="#"><i class="fa fa-facebook"></i></a>
                                                        <a href="#"><i class="fa fa-google"></i></a>
                                                    </div>

                                                </div>
                                            </form>
                                        </div>
                                        <div role="tabpanel" class="tab-pane" id="signup">
                                            <form class="form-m" id="registerform" @submit.prevent="submitForm">
                                                <mdb-input type="text" label="Enter your first name" outline />

                                                <mdb-input type="text" label="Enter your last name" outline />

                                                <mdb-input type="email" label="Enter your email" outline />

                                                <mdb-input type="password" label="Enter your password" outline />

                                                <div class="row">
                                                    <div class="col-md-12">
                                                        <div class="checkbox">
                                                            <label class="check-label">
                                                                <input type="checkbox"> I have agreed to the <a
                                                                    class="terms" href="">terms and conditions </a>of
                                                                peexo.ai
                                                            </label>
                                                        </div>
                                                    </div>

                                                </div>
                                                <div class="row text-center" style="margin-top:20px">
                                                    <div class="col-md-6 offset-md-3">
                                                        <button class="btn btn-rounded btn-peexoo text-white">SIGN
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
                                            </form>
                                        </div>
                                    </div>
                                </div>
                            </div>

                        </div>
                    </div>
                </div>
            </div>
        </div>
    </transition>
</div>
  
</template>
<script>
    import modal from './confirm-password'
    import { mdbInput } from 'mdbvue';
    export default {
        name: 'login-register-modal',
        props: ['show'],
        components: {
            modal,
            mdbInput
        },
        data: function () {
            return {
                loginForm: {
                    email: '',
                    password: ''
                },
                registerForm: {
                    email: '',
                    password: '',
                    // password_confirmation: '',
                    first_name: '',
                    last_name: '',
                },
                showloginModal: false,
                showConfirmPasswordModal: false,
                loading: true
            }
        },
        mounted: function () {
            // console.log('first time component :' + this.show)
            // //console.log('After click :' + this.show)
            // document.addEventListener("keydown", (e) => {
            //     if (this.showloginModal && e.keyCode == 27) {
            //         this.close();
            //     }
            // });
            
        },
        methods: {
            close: function () {
                this.$emit('close');
            },
            // login(e) {
            //     // axios.post('/api/auth/login', this.loginForm).then(response => {
            //     //     localStorage.setItem('auth_token', response.data.token);
            //     //     axios.defaults.headers.common['Authorization'] = 'Bearer ' + localStorage.getItem('auth_token');
            //     //     toastr['success'](response.data.message);
            //     //     this.$router.push('/home')
            //     // }).catch(error => {
            //     //     toastr['error'](error.response.data.message);
            //     // });
                
            // },
            submitForm(e) {
                // axios.post('/api/auth/register', this.registerForm).then(response => {
                //     toastr['success'](response.data.message);
                //     //this.$router.push('/user');
                // }).catch(error => {
                //     toastr['error'](error.response.data.message);
                // });
                this.close();
                this.showConfirmPasswordModal = true
            },
        }

    }
</script>
<style scoped>
    .modal-mask {
        position: fixed;
        z-index: 9998;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-color: rgba(0, 0, 0, .5);
        transition: opacity .3s ease;
    }

    /*
 * The following styles are auto-applied to elements with
 * transition="modal" when their visibility is toggled
 * by Vue.js.
 *
 * You can easily play with the modal transition by editing
 * these styles.
 */

    .modal-enter {
        opacity: 0;
    }

    .modal-leave-active {
        opacity: 0;
    }

    .modal-enter .modal-container,
    .modal-leave-active .modal-container {
        -webkit-transform: scale(1.1);
        transform: scale(1.1);
    }

    .modal-container {
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background: rgba(0, 0, 0, 0.3) !important;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    #confirm-modal {
        background: #fefbf3;
    }

    .close-btn {
        position: absolute;
        right: -1rem;
        top: -1rem;
        z-index: 1000;
        background: #d8d8d8;
        border-radius: 50%;
        height: 40px;
        width: 40px;
        color: #4f4f4f;
        font-weight: normal;
        padding: 10px 12px;
    }

    .fa-times {
        font-size: 20px;
    }

    .li-m {
        padding-top: 15px;
        text-align: center;
        background: #fefbf3;
        justify-content: normal;
    }

    .li-m a {
        padding: 18px 73px;

    }

    a.active {
        background: #ffb503
    }

    .form-m {
        padding: 44px 40px 27px 40px;
        background: #fefbf3;
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
        padding: 8px 12px 1px 12px;
        border-radius: 50%;
        color: #fff;
        height: 33px;
        margin-right: 10px;
    }

    .fa-google {
        background: #db4a39;
        padding: 8px 9px 0px 11px;
        border-radius: 50%;
        color: #fff;
        height: 33px;

    }

    .terms {
        color: #be7e00 !important;
        font-family: 'Montserrat';
    }
</style>