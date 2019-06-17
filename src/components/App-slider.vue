<template>
    <canvas id="kenburns">
        <p>Your browser doesn't support canvas!</p>
    </canvas>
</template>
<script>
    import axios from 'axios'
    export default {
        data: function () {
            return {
                images: [
                        'http://www.kelechiamadiobi.com/wp-content/uploads/2015/06/slider-4.jpg',
                        'https://mdbootstrap.com/img/Photos/Slides/img%20(6).jpg',
                        'https://mdbootstrap.com/img/Photos/Slides/img%20(9).jpg'   
                ],
                
                timer: null
            }
        },
        mounted: function () {
                var $canvas = jQuery('#kenburns');
                $canvas.attr('width', jQuery(window).width());
                $canvas.attr('height', jQuery(window).height());

                $canvas.kenburned({
                    images: this.images,
                    frames_per_second: 100,
                    display_time: 7000,
                    zoom: 1.2,
                    fade_time: 1000,
                });
        },
        components: {
            
        },
        methods: {
        // created(){
                //     // axios.get('https://jsonplaceholder.typicode.com/photos?_limit=5')
                //     //     .then(res => res.data.forEach((img) => {
                //     //         this.images.push(img.url)})
                //     //     )
                //     //     .catch(err => console.log(err))
                // }
        },

       
    }
</script>
<style scoped>
    .im {
        width: 100%;
    }
</style>