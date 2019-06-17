<template>
    <mdb-row>
        <mdb-card>
            <mdb-view hover>
                <a href="#!">
                    <mdb-card-image src="https://mdbootstrap.com/img/Photos/Others/images/16.jpg" alt="Card image cap">
                    </mdb-card-image>
                    <mdb-mask flex-center waves overlay="white-slight"></mdb-mask>
                </a>
            </mdb-view>
            <mdb-card-body>
                <mdb-card-title :username="username">{{username}}</mdb-card-title>
                <mdb-card-text :desc="desc">{{desc}}</mdb-card-text>
                <button style="color:#fff" class="btn btn-p btn-rounded btn-peexoo">Book now</button>
            </mdb-card-body>
        </mdb-card>
    </mdb-row>
</template>
<script>
    import {mdbRow, mdbCol, mdbCard, mdbCardImage,mdbCardBody, mdbCardTitle, mdbCardText,mdbView, mdbMask } from 'mdbvue';

    export default {
        name: 'card-list',
        props: ['username', 'desc'],
        components: {
            mdbRow,
            mdbCol,
            mdbCard,
            mdbCardImage,
            mdbCardBody,
            mdbCardTitle,
            mdbCardText,
            mdbView,
            mdbMask
        }
    }
</script>