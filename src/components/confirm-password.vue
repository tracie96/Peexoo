<template>
    <transition name="modal">
        <div class="modal-mask" v-show="show">
            <div class="modal-container">
                <div class="modal-dialog" role="document">
                    <div class="modal-content">
                        <div class="alert-contain">
                            <h5>Confirm your email</h5>
                            <p class="text-center text-inside">
                                A verification link and code has been sent to your email, click on the link or use the
                                code to
                                confirm your email instantly.
                            </p>
                            <div class="container">
                                <div class="login-flex-parent" style="margin: 38px 0px 38px 0px;">
                                    <div class="flex-child-edge"></div>
                                    <div class="login-flex-child-text log">enter code below</div>
                                    <div class="flex-child-edge"></div>
                                </div>
                                <security-code v-model="code"></security-code>
                                <div class="text-center">
                                    <button style="color:#fff" class="btn btn-p btn-rounded btn-peexoo">ENTER CODE</button>
                                </div>
                               
                            </div>


                        </div>
                    </div>
                </div>
            </div>
        </div>
    </transition>

</template>

<script>
    import SecurityCode from 'vue-security-code'
    export default {
        name: "confirm-password",
        props: ['show'],
        components: { SecurityCode },

        data: function () {
            return {
                code: ''
            }
        },
        mounted: function () {
            document.addEventListener("keydown", (e) => {
                if (this.show && e.keyCode == 27) {
                    this.close();
                }
            });
        },
        methods: {
            close: function () {
                this.$emit('close');
            }
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

    .modal-content {
        padding-left: 30px !important;
        padding-right: 30px !important;
    }
    .log {
        color: #b58000 !important;
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

    .alert-contain h5 {
        font-family: Lora;
        font-size: 36px;
        font-weight: normal;
        font-style: normal;
        font-stretch: normal;
        line-height: normal;
        letter-spacing: normal;
        text-align: center;
        color: #4d4d4d !important;
        padding-top: 81px;
    }

    .alert-contain p.text-inside {
        font-family: 'Montserrat';
        font-size: 16px;
        font-weight: normal;
        font-style: normal;
        font-stretch: normal;
        line-height: normal;
        letter-spacing: normal;
        text-align: center;
        color: #4d4d4d !important;
        padding: 35px 40px 0 40px;
    }
</style>