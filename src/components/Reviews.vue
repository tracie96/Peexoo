<template>
    <div class="row" style="margin-bottom:29px">
        <div class="col-md-3 user-details">
            <img :src="getImgUrl(img)" :img="img" alt="">
                <span :photoname="photoname">{{photoname}}</span> <br>
                <span id="date" :date="date">{{date}}</span> <br>
                <span id="star-icons">
                    <i class="fa peexo-body-text fa-star"></i> <i class="fa peexo-body-text fa-star"></i> <i class="fa peexo-body-text fa-star"></i> <i class="fa peexo-body-text fa-star"></i> <i class="fa peexo-body-text fa-star"></i>
                </span>

        </div>
         <div class="col-md-9">
            <p class="peexo-body-text" :revbody="revbody">
                 {{revbody}}
            </p>
        </div>
    </div>
</template>
<script>
export default {
    name:"reviews",
    props: ['revbody','img', 'photoname', 'date'],
    methods: {
    getImgUrl(img) {
        return require('../assets/' + img)
    }
  }
}
</script>

 <style scoped>
 .user-details span{
    color: #4d4d4d !important;
    padding-left: 20px;
    position: relative;
    top: -10px;
    font-weight: normal !important;
 }
 #date, #star-icons{
    color: #4d4d4d !important;
    padding-left: 97px;
    position: relative;
    left: -14px;
    top: -28px;
    font-weight: normal !important;
 }
 
 </style>
 