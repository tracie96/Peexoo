<template>
    <div class="black-header">
            <h3>Join the Community</h3>
            <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
                dolore magna aliqua.
            </p>
            <router-link class="" to="/community/join">
                    <button class="btn btn-p btn-rounded btn-peexoo">Join the Community</button>
            </router-link>
            
        </div>
</template>

<style scoped>
 .black-header {
        height: 475px !important;
    }

    .black-header p {
        padding: 10px 350px 10px 350px;
        font-weight: normal !important
    }
     @media (max-width: 480px) {
         
        .black-header p {
        padding: 10px;
         
        }
        
    }
</style>
