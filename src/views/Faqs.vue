<template>
    <div>
        <PHeader />
        <div class="desktop">
            <div class="black-header">
                <h3>FAQs</h3>
                <p>
                    Got any questions?
                </p>
            </div>
            <div class="row body-div">
                <div class="col-md-2">
                    <ul class="mg-top">
                        <a href="#">
                            <li v-on:click="billing" class="list-group-item">Billing</li>
                        </a>
                        <a href="#">
                            <li v-on:click="reg" class="list-group-item">Registration</li>
                        </a>
                        <a href="#">
                            <li class="list-group-item">Billing</li>
                        </a>
                        <a>
                            <li class="list-group-item">Billing </li>
                        </a>
                        <a>
                            <li class="list-group-item">Billing </li>
                        </a>
                    </ul>
                </div>
                <div class="col-md-9" id="billing" v-if="isBilling">
                    <div id="accordion" class="mg-top">
                        <p>
                            Billing
                        </p>
                        <div class="card">

                            <div class="card-header" id="headingOne">
                                <h5 class="mb-0">
                                    <a href="#" class="expand-text" data-toggle="collapse" data-target="#collapseOne"
                                        aria-expanded="true" aria-controls="collapseOne">
                                        Collapsible Group Item #1 <i class="fa fa-angle-down rotate-icon"></i>
                                    </a>
                                </h5>
                            </div>

                            <div id="collapseOne" class="collapse show" aria-labelledby="headingOne"
                                data-parent="#accordion">
                                <div class="card-body">
                                    Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry
                                    richardson ad
                                    squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck
                                    quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor, sunt aliqua put a bird
                                    on it
                                    squid single-origin coffee nulla assumenda shoreditch et. Nihil anim keffiyeh
                                    helvetica,
                                    craft beer labore wes anderson cred nesciunt sapiente ea proident. Ad vegan
                                    excepteur
                                    butcher vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic
                                    synth
                                    nesciunt you probably haven't heard of them accusamus labore sustainable VHS.
                                </div>
                            </div>
                        </div>
                        <div class="card">
                            <div class="card-header" id="headingTwo">
                                <h5 class="mb-0">
                                    <a href="#" class=" collapsed" data-toggle="collapse" data-target="#collapseTwo"
                                        aria-expanded="false" aria-controls="collapseTwo">
                                        Collapsible Group Item #2 <i class="fa fa-angle-down rotate-icon"></i>
                                    </a>
                                </h5>
                            </div>
                            <div id="collapseTwo" class="collapse" aria-labelledby="headingTwo"
                                data-parent="#accordion">
                                <div class="card-body">
                                    Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry
                                    richardson ad
                                    squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck
                                    quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor, sunt aliqua put a bird
                                    on it
                                    squid single-origin coffee nulla assumenda shoreditch et. Nihil anim keffiyeh
                                    helvetica,
                                    craft beer labore wes anderson cred nesciunt sapiente ea proident. Ad vegan
                                    excepteur
                                    butcher vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic
                                    synth
                                    nesciunt you probably haven't heard of them accusamus labore sustainable VHS.
                                </div>
                            </div>
                        </div>
                        <div class="card">
                            <div class="card-header" id="headingThree">
                                <h5 class="mb-0">
                                    <a href="#" class="collapsed" data-toggle="collapse" data-target="#collapseThree"
                                        aria-expanded="false" aria-controls="collapseThree">
                                        Collapsible Group Item #3 <i class="fa fa-angle-down rotate-icon"></i>
                                    </a>
                                </h5>
                            </div>
                            <div id="collapseThree" class="collapse" aria-labelledby="headingThree"
                                data-parent="#accordion">
                                <div class="card-body">
                                    Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry
                                    richardson ad
                                    squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck
                                    quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor, sunt aliqua put a bird
                                    on it
                                    squid single-origin coffee nulla assumenda shoreditch et. Nihil anim keffiyeh
                                    helvetica,
                                    craft beer labore wes anderson cred nesciunt sapiente ea proident. Ad vegan
                                    excepteur
                                    butcher vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic
                                    synth
                                    nesciunt you probably haven't heard of them accusamus labore sustainable VHS.
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-md-9" id="reg" v-if="isReg">
                    <div id="accordion" class="mg-top">
                        <p>
                            Registration
                        </p>
                        <div class="card">

                            <div class="card-header" id="headingOne">
                                <h5 class="mb-0">
                                    <a href="#" class="" data-toggle="collapse" data-target="#collapseOne"
                                        aria-expanded="true" aria-controls="collapseOne">
                                        Collapsible Group Item #1 <i class="fa fa-angle-down rotate-icon"></i>
                                    </a>
                                </h5>
                            </div>

                            <div id="collapseOne" class="collapse show" aria-labelledby="headingOne"
                                data-parent="#accordion">
                                <div class="card-body">
                                    Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry
                                    richardson ad
                                    squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck
                                    quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor, sunt aliqua put a bird
                                    on it
                                    squid single-origin coffee nulla assumenda shoreditch et. Nihil anim keffiyeh
                                    helvetica,
                                    craft beer labore wes anderson cred nesciunt sapiente ea proident. Ad vegan
                                    excepteur
                                    butcher vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic
                                    synth
                                    nesciunt you probably haven't heard of them accusamus labore sustainable VHS.
                                </div>
                            </div>
                        </div>
                        <div class="card">
                            <div class="card-header" id="headingTwo">
                                <h5 class="mb-0">
                                    <a href="#" class=" collapsed" data-toggle="collapse" data-target="#collapseTwo"
                                        aria-expanded="false" aria-controls="collapseTwo">
                                        Collapsible Group Item #2 <i class="fa fa-angle-down rotate-icon"></i>
                                    </a>
                                </h5>
                            </div>
                            <div id="collapseTwo" class="collapse" aria-labelledby="headingTwo"
                                data-parent="#accordion">
                                <div class="card-body">
                                    Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry
                                    richardson ad
                                    squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck
                                    quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor, sunt aliqua put a bird
                                    on it
                                    squid single-origin coffee nulla assumenda shoreditch et. Nihil anim keffiyeh
                                    helvetica,
                                    craft beer labore wes anderson cred nesciunt sapiente ea proident. Ad vegan
                                    excepteur
                                    butcher vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic
                                    synth
                                    nesciunt you probably haven't heard of them accusamus labore sustainable VHS.
                                </div>
                            </div>
                        </div>
                        <div class="card">
                            <div class="card-header" id="headingThree">
                                <h5 class="mb-0">
                                    <a href="#" class="collapsed" data-toggle="collapse" data-target="#collapseThree"
                                        aria-expanded="false" aria-controls="collapseThree">
                                        Collapsible Group Item #3 <i class="fa fa-angle-down rotate-icon"></i>
                                    </a>
                                </h5>
                            </div>
                            <div id="collapseThree" class="collapse" aria-labelledby="headingThree"
                                data-parent="#accordion">
                                <div class="card-body">
                                    Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry
                                    richardson ad
                                    squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck
                                    quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor, sunt aliqua put a bird
                                    on it
                                    squid single-origin coffee nulla assumenda shoreditch et. Nihil anim keffiyeh
                                    helvetica,
                                    craft beer labore wes anderson cred nesciunt sapiente ea proident. Ad vegan
                                    excepteur
                                    butcher vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic
                                    synth
                                    nesciunt you probably haven't heard of them accusamus labore sustainable VHS.
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="for-mobile">
            <h3>
                FAQs
            </h3>
            <div class="row">
                <div class="col-6" v-for="(faq, key) in Faqs" :key="key">
                    <div class="card faq-card-item">
                       <router-link class="log" :to="{path: '/faqs/mobile/' + faq.id }">{{faq.title}}</router-link> 
                    </div>
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
    export default {
        name: "faqs",
        data: function () {
            return {
                isBilling: true, isReg: false,
                Faqs: [
                    {
                        id: 1,
                        title:"Billing"
                    },
                    {   
                        id:2,
                        title:"Registration"
                    },
                    {
                        id:3,
                        title:"Something"
                    },
                    {
                        id:4,
                        title:"Billing"
                    },
                    {
                        id:5,
                        title:"Billing"
                    },
                    {
                        id:6,
                        title:"Billing"
                    }
                     
                ]
            }
        },
        components: {
            PHeader,
            Footer,
            Menu
        },
        methods: {
            billing() {
                this.isBilling = true
                this.isReg = false
            },
            reg() {
                this.isBilling = false
                this.isReg = true
            }
        }
    }
</script>
<style scoped>
.card{
    box-shadow: none !important;
}
    @media screen and (max-width: 560px) {
        .for-mobile {
            display: block !important
        }

        .desktop {
            display: none
        }

        .for-mobile {
            margin-top: 100px;
            padding-left: 22px;
            padding-right: 22px;
            margin-bottom: 50px
        }
        .col-6{
            padding-right: 8px !important;
            padding-left: 8px !important;
            margin-bottom: 10px
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

        .faq-card-item {
            height: 91px;
            text-align: center;
            padding-top: 38px;
            border-radius: 5px;
            font-size: 16px;
            box-shadow: 0 3px 12px -2px rgba(223, 223, 223, 0.5);
            background-color: #ffffff;
        }
        
         
    }

    .for-mobile {
        display: none
    }
    .mb-0 a.collapsed{
        color: #474747 !important;
    }
     
    .body-div {
        margin-bottom: 200px
    }

    a {
        color: #474747 !important
    }

    a:hover {
        color: #7b7a76 !important;
        text-decoration: none;
    }

    .side-list {
        margin-top: 154px
    }

    .list-group-item {
        background-color: #fefbf3 !important;
        border: none !important;
        margin-left: 40px
    }

    .mg-top {
        margin-top: 60px
    }

   
    #accordion {
        border-left: 1px solid #979797;
    }

    #accordion p {
        padding: .75rem 2.25rem;
        font-family: Lora;
        font-size: 36px;
        font-weight: normal;
        font-style: normal;
        font-stretch: normal;
        line-height: normal;
        letter-spacing: normal;
        color: #474747;
    }

   

    .card-header,
    .card-body {
        background: rgb(254, 251, 243) !important
    }

    .card-body {
        padding: 2.25rem !important;
    }

    .card-header {
        border-bottom: none !important;
        font-size: 18px;
        padding: .75rem 2.25rem !important;
    }

    .card {
        border: none !important;
    }
    .mb-0 a {
        color: #ffb503 !important;
        font-family: 'Montserrat'
    }
    .mb-0 {
        border-bottom: solid 0.5px #979797;
        padding-bottom: 25px;
    }
    
    .card .card-header a:not(.collapsed) .rotate-icon {
        -webkit-transform: rotate(180deg);
        -ms-transform: rotate(180deg);
        transform: rotate(180deg);
    }
    .card .fa-angle-down {
        float: right;
        color: #474747 !important;
        font-size: 25px;
    }
</style>