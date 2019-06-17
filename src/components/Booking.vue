<template>
     <section class="">
        <div class="container">
            <div class="row">
                <div class="col-lg-10 mx-auto">
                    <div class="agency-section-title t2 text-center section-title-style2">
                        <h2 class="main-title" style="color:#ffb503">What kind of Booking do you want?</h2>
                        <p class="p-italics">
                            Select a particular style of photoshoot/videoshoot to book
                        </p>
                    </div>
                </div>
            </div><!-- .row end -->
            <div class="row">
                <div class="col-md-6 col-lg-3 col-6" v-for="(booking, key) in Bookings" :key="key">
                    <div class="single-info-block text-center">
                        <div class="info-header">
                            <img :src="require(`../assets/images/${booking.img}`)">
                        </div>
                        <p>{{booking.caption}} </p>
                    </div><!-- .single-info-block END -->
                </div>
                 
            </div><!-- .row END -->
             <div class="row more-book" v-if="!isHidden">
                <div class="col-md-6 col-lg-3 col-6" v-for="(booking, key) in MmoreBookings" :key="key">
                    <div class="single-info-block text-center">
                        <div class="info-header">
                            <img :src="require(`../assets/images/${booking.img}`)">
                        </div>
                        <p>{{booking.caption}} </p>
                    </div><!-- .single-info-block END -->
                </div>
                 
            </div><!-- .row END -->
             
            <p v-on:click="isHidden = !isHidden" id="show-more" class="text-center pad-top-40 show-special" v-if="isHidden">
                 Show more Specialties
            </p>
             <p v-on:click="isHidden = !isHidden" id="show-more" class="text-center pad-top-40 show-special" v-if="!isHidden">
                Hide Specialties
            </p>
            <p class="text-center">
                <i v-if="isHidden" class="show-icon bounce fa-x fa fa-chevron-circle-down"></i>
            </p>
        </div><!-- .container END -->
    </section><!-- end business info section -->
</template>


<script>
export default {
    data(){
        return{
            isHidden: true,
            Bookings : [
            {
                img:'thelexash-59052115-633195593820735-5160150945884080536-n.png',
                caption: 'Portrait'
            },
            {
                img:'afroshots-28153960-1915701772073569-3293591341610565632-n.png',
                caption: 'Events'
            },{
                img:'burgerking-58887042-393547187897733-2860389474261161166-n.png',
                caption: 'Product'
            },{
                img:'gtbank-picture-test-3.png',
                caption: 'Real Estate'
            } 
        ],
           MmoreBookings : [
            {
                img:'thelexash-59052115-633195593820735-5160150945884080536-n.png',
                caption: 'Portrait'
            },
            {
                img:'afroshots-28153960-1915701772073569-3293591341610565632-n.png',
                caption: 'Events'
            },{
                img:'burgerking-58887042-393547187897733-2860389474261161166-n.png',
                caption: 'Product'
            },{
                img:'gtbank-picture-test-3.png',
                caption: 'Real Estate'
            } 
        ]
        }
    }
}
</script>
<style scoped>
.more-book{
    margin-top:25px;
    overflow:auto;
    transition: max-height 0.5s, overflow 0.5s 0.5s;
    animation: fade 1s;
}
@keyframes fade {
    0% {
        opacity: 0;
    }

    100% {
        opacity: 1;
    }
}
 .t2 .main-title{
    font-size:40px !important
    }
    @media (max-width: 480px) {
        .t2 .main-title{
    font-size:28px !important
    }
    }
</style>
