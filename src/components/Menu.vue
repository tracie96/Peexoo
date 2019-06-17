<template>
    <div id="footer-menu" class="footer-menu-3-icons footer-menu-style-1">
            <a href="#" class="active-nav">
                <img src="../assets/images/photographer.svg" alt="">
                <span>Find Photographers</span>
            </a>
            <a href="#">
                <img src="../assets/images/portrait.svg" alt="">
                <span>Find my Photos</span>
            </a>
            <a href="#">
                 <img src="../assets/images/photo-copy.svg" alt="">
                <span>Explore Photos</span>
            </a>
            <div class="clear"></div>
    </div>
</template>
 <style scoped>
   a,
    b,
    div,
    li,
    ul {
        -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
        -webkit-tap-highlight-color: transparent;
        -moz-outline-: none;
        position: relative;
        
    }
    @media only screen and (min-width: 320px) and (max-width: 420px) {
    .single-info-block {
        min-height: 225px;
    }
    
     #footer-menu a span {
        left: 0;
        right: 0;
        font-weight: 600;
        font-size: 11px;
        padding: 48px 0px 16px 9px;
        }
    #footer-menu a img{
        
        padding-top: 15px !important;
    }
    }
    @media  (max-width: 480px) {
    .single-info-block {
        min-height: 225px;
    }
    
     #footer-menu a span {
        left: 0;
        right: 0;
        font-weight: 600;
        font-size: 11px;
        padding: 48px 0px 16px 9px;
    }
    }
 </style>
 