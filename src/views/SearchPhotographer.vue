<template>
    <div>
        <PHeader />
        <div class="container">
            <div class="row mt-15">
                <div class="col-md-4">
                    <div class="container">
                        <div class="">
                            <div class="inner-addon right-addon">
                                <i class="fa fa-search"></i>
                                <input type="text" class="form-control" placeholder="Search" />
                            </div>
                        </div>

                        <p class="p-title-category">
                            Category Type
                        </p>
                        <div>
                            <Searchcategory :name="category.name" v-for="(category, key) in Categories" :key="key" />
                        </div>

                        <p class="p-title-category">
                            Photographer Type
                        </p>
                        <div>
                            <Searchtype :name="type.name" v-for="(type, id) in Types" :key="id" />
                        </div>

                        <p class="p-title-category">
                            Bases Region
                        </p>
                        <h6>Seperate with a comma</h6>
                        <p class="p-title-category">
                            Price
                        </p>
                        <RangeSlider />
                        <p class="p-title-category">
                            Availability
                        </p>
                        <v-layout wrap>
                            <v-flex sm6 md6>
                                <v-menu v-model="menu2" :close-on-content-click="false" :nudge-right="40" lazy
                                    transition="scale-transition" offset-y full-width>
                                    <template v-slot:activator="{ on }">
                                        <v-text-field v-model="date" label="From" readonly v-on="on"></v-text-field>
                                    </template>
                                    <v-date-picker v-model="date" color="green lighten-1" @input="menu2 = false">
                                    </v-date-picker>
                                </v-menu>
                            </v-flex>
                            <v-flex sm6 md6>
                                <v-menu v-model="menu2" :close-on-content-click="false" :nudge-right="40" lazy
                                    transition="scale-transition" offset-y full-width>
                                    <template v-slot:activator="{ on }">
                                        <v-text-field v-model="date" label="To" readonly v-on="on"></v-text-field>
                                    </template>
                                    <v-date-picker v-model="date" color="green lighten-1" @input="menu2 = false">
                                    </v-date-picker>
                                </v-menu>
                            </v-flex>
                        </v-layout>
                        <div class="advert">
                            <img src="../assets/images/app-screen-mockup.png" alt="peexoo apps">
                            <p class="text-white">
                                    DON’T MISS OUT!
                                    DOWNLOAD OUR MOBILE APP
                                    FOR A FULL MOBILE
                                    EXPERIENCE
                            </p>
                            <div class="pad-top-30 text-center">
                                    <div>
                                      <img style="width:70%" src="../assets/images/ww_app-store.png" alt="download from app store">
                                    </div>
                                    <div>
                                      <img style="width:78%" src="../assets/images/google-play.png" alt="download from google store">
                                    </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-md-8">
                    <h4>320 Photograhers found</h4>
                    <div class="row">

                        <div class="col-md-6" v-for="(card, key) in Photographers" :key="key">
                            <Cardlist :username="card.username" :desc="card.desc" />
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <Footer/>
        <Menu/>
    </div>


</template>
<script>
    import PHeader from '../components/PHeader'
    import Footer from '../components/Footer'
    import Menu from '../components/Menu'
    import Cardlist from '../components/card-list'
    import Searchcategory from '../components/search-category'
    import Searchtype from '../components/search-type'
    import RangeSlider from '../components/range-slider'


    export default {

        components: {
            PHeader,
            Footer,
            Menu,
            Cardlist,
            Searchcategory,
            Searchtype,
            RangeSlider

        },
        data: function () {
            return {
                date: new Date().toISOString().substr(0, 10),
                menu2: false,
                Photographers: [
                    {
                        id: 1,
                        username: 'Jeremiah Abimbola',
                        desc: 'There is a reason that I am called the god of photographer. I shoot the invicible and',
                    },
                    {
                        id: 2,
                        username: 'Tolulope Wsbdsd',
                        desc: 'There is a reason that I am called the god of photographer. I shoot the invicible and',
                    },
                    {
                        id: 3,
                        username: 'Wale Tinubu',
                        desc: 'There is a reason that I am called the god of photographer. I shoot the invicible and',
                    },
                    {
                        id: 4,
                        username: 'dbashdjbfajhsdfj hasdjf',
                        desc: 'There is a reason that I am called the god of photographer. I shoot the invicible and…',
                    },
                    {
                        id: 5,
                        username: 'Wale Tinubu',
                        desc: 'There is a reason that I am called the god of photographer. I shoot the invicible and',
                    },
                    {
                        id: 6,
                        username: 'dbashdjbfajhsdfj hasdjf',
                        desc: 'There is a reason that I am called the god of photographer. I shoot the invicible and…',
                    },
                    {
                        id: 7,
                        username: 'Wale Tinubu',
                        desc: 'There is a reason that I am called the god of photographer. I shoot the invicible and',
                    },
                    {
                        id: 8,
                        username: 'dbashdjbfajhsdfj hasdjf',
                        desc: 'There is a reason that I am called the god of photographer. I shoot the invicible and…',
                    }
                ],
                Categories: [
                    {
                        id: 1,
                        name: 'Portrait'
                    },
                    {
                        id: 2,
                        name: 'Events'
                    },
                    {
                        id: 3,
                        name: 'Real Estate'
                    }
                ],
                Types: [
                    {
                        id: 1,
                        name: 'Select all'
                    },
                    {
                        id: 2,
                        name: 'Still picture (photo)'
                    },
                    {
                        id: 3,
                        name: 'Motion picture (video)'
                    }
                ]
            }
        }
    }
</script>
<style scoped>
    .advert{
        padding: 20px;
        margin-top:20px;
        width: 97%;
        height: 700px;
        background-image: linear-gradient(to bottom, rgba(255, 255, 255, 0.5), #ffb400 43%, #ffb503), linear-gradient(to bottom, #ffb503, #ffb503);
    }
    .advert p{
        font-family: Lora;
        font-size: 28px;
        font-weight: bold;
        font-style: normal;
        font-stretch: normal;
        line-height: normal;
        letter-spacing: normal;
        text-align: center;
        color: #ffffff;
        margin-top:20px
    }
    .p-title-category {
        font-family: 'Montserrat';
        font-size: 18px;
        font-weight: 600;
        font-style: normal;
        font-stretch: normal;
        line-height: normal;
        letter-spacing: normal;
        color: #4d4d4d;
        margin-top: 28px
    }

    h4 {
        font-family: 'Montserrat' !important;
        font-size: 24px !important;
        font-weight: normal !important;
        color: #4d4d4d !important;
        margin-left: -15px !important;
        margin-bottom: 20px
    }

    /* enable absolute positioning */
    .inner-addon {
        position: relative;
    }

    /* style glyph */
    .inner-addon .fa {
        position: absolute;
        padding: 10px;
        pointer-events: none;
    }

    .right-addon .fa {
        right: 0px;
    }


    .right-addon input {
        padding-right: 30px;
    }
</style>