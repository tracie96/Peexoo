<template>
    <div>
        <PHeader />
        <div class="row">
            <div class="for-mobile">
                <h3>
                    FAQs / {{title}}
                </h3>

                <div style="float:right">
                    <router-link class="back" to="/faqs">
                       Back to FAQs</router-link> </div> <br> <br>

                            <div class="col-12">
                                <accordion :panes="panes" material></accordion>
                            </div>
                </div>
            </div>
            <Footer />
            <Menu />
        </div>
</template>

<script>
    import PHeader from '../components/PHeader'
    import Footer from '../components/Footer'
    import Menu from '../components/Menu'
    import { Accordion } from 'mdbvue';
    export default {
        name: "mobilefaqs",
        data: function () {
            return {
                title: '',
                panes: [],
            }
        },
        components: {
            PHeader,
            Footer,
            Menu,
            Accordion
        },
        methods: {

        },
        mounted() {
            var url = document.URL;
            var id = url.substring(url.lastIndexOf('/') + 1);
            if (id == 1) {
                this.title = 'Billing'
                var obj = {}
                obj.title = "Lorem ipsum dolor sit amet, consectetur adipiscing elit,"
                obj.content = "lorem dfasdhfjhsd asdhfjhsdgfj gasjdhfgajshdgf jgasdhfgjashdgf agshdfasdf sdf "
                this.panes.push(obj);
                var obj2 = {}
                obj2.title = "Lorem ipsum dolor sit amet, consectetur adipiscing elit"
                obj2.content = "lorem two dfasdhfjhsd asdhfjhsdgfj gasjdhfgajshdgf jgasdhfgjashdgf agshdfasdf sdf "
                this.panes.push(obj2);
            }
            else if (id == 2) {
                this.title = 'Registration'
                var obj = {}
                obj.title = "Lorem ipsum dolor sit amet, consectetur adipiscing elit,"
                obj.content = "lorem dfasdhfjhsd asdhfjhsdgfj gasjdhfgajshdgf jgasdhfgjashdgf agshdfasdf sdf "
                this.panes.push(obj);
                var obj2 = {}
                obj2.title = "Lorem ipsum dolor sit amet, consectetur adipiscing elit"
                obj2.content = "lorem two dfasdhfjhsd asdhfjhsdgfj gasjdhfgajshdgf jgasdhfgjashdgf agshdfasdf sdf "
                this.panes.push(obj2);
            }
            
        },

    }
</script>

<style>
    .for-mobile {
        display: none
    }

    @media screen and (max-width: 560px) {
        .back{
            color:#b58000
        }
        .for-mobile {
            display: block !important;
        }
        .accordion .card{
            margin-bottom: 20px !important;
        }
        .fas{
            float:right;
            color: #474747;
        }
        .accordion .card-header{
            background: #fff !important;
            border-bottom: none !important;
        
        }
        .accordion  .card-body{
           font-size: 14px
        }
        .accordion .mb0 span{
            font-size:16x
        }
        .accordion .card-header a h5{
            color:#ffb600 !important;
        }
        .for-mobile {
            margin-top: 100px;
            padding-left: 30px;
            padding-right: 30px;
            margin-bottom: 50px
        }

        .for-mobile h3 {
            font-family: Lora;
            font-size: 24px;
            font-weight: bold;
            font-style: normal;
            font-stretch: normal;
            line-height: normal;
            letter-spacing: normal;
            color: #414141;
            margin-bottom: 30px
        }
    }
</style>