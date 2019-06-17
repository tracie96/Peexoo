<template>
    <v-app>
      <div class="slid">
        N <span >{{price[0]}}</span> - N <span >{{price[1]}}</span>
        <v-range-slider color="peexoo" v-model="price" :max="300000" :min="0" :step="10"></v-range-slider>
      </div>
    </v-app>
</template>

<script>
  export default {
    name: 'range-slider',
    data() {
      return {
        price: [35630, 136880]
      }
    }
  }
</script>
<style >
.slid > span{
  font-size: 14px !important;
   font-family: 'Montserrat' !important;
  font-weight: normal;
  font-style: normal;
  font-stretch: normal;
  line-height: normal;
  letter-spacing: normal;
  color: #4d4d4d !important;
}
.v-slider__track__container{
  background: #efefef !important;
  height: 7px;
  border-radius: 3px;
}
.theme--light.v-input--slider .v-slider__track{
   background: #efefef !important;
}
.v-slider__track-fill{
  height: 7px !important;
  background: #ffb504 !important
}
.v-slider__thumb{
  box-shadow: 0 2px 4px 0 rgba(119, 119, 119, 0.5) !important;
  padding: 13px !important;
  border: 0.5px solid #c7c6c2 !important;
  
}
.peexoo {
    background-color: #fff ;
}
.v-messages{
  display: none !important;
}
.peexoo--text {
    color: #fff !important;
    caret-color: #fff !important;
}
</style>
