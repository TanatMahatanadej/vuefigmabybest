<template>
    <div class="home">
        <div class="navbar">
            <div class="logo">Logo</div>
            
            <div class="menu">
                <div class="trip" >Trip</div>
                <div class="blog" >Blog</div>
                <div class="faq">FAQ</div>
                <div class="contact" >Contact</div>
                <div class="logingroup">
                    <img src="../../picture/Vector.jpg" style="display:flex;"/>
                    <div class="login">Log in</div>
                </div>
            </div>
        </div>

        <div class="rectangle2">
            <div class="rectopic">
                Lorem ipsum dolor sit amet
            </div>
            <div class="p1">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit.
            </div>
            <div class="birdcontainer">
                <!-- <div class="item" v-for="(item,i) in items" :key="i" >
                    
                </div> -->
                <!-- <div class="imgborder" style="width: 169.95px; height:136px">
                    <img src="../../picture/imagebird.jpg" alt="pic" style="border-radius:50%; width:136px; height:136px" >
                    <div class="caption">Lorem ipsum</div>
                </div>
                <div class="imgborder" style="width: 169.95px; height:136px">
                    <img src="../../picture/imagebird.jpg" alt="pic" style="border-radius:50%; width:136px; height:136px" >
                    <div class="caption">Lorem ipsum</div>
                </div>
                <div class="imgborder" style="width: 169.95px; height:136px">
                    <img src="../../picture/imagebird.jpg" alt="pic" style="border-radius:50%; width:136px; height:136px" >
                    <div class="caption">Lorem ipsum</div>
                </div>
                <div class="imgborder" style="width: 169.95px; height:136px">
                    <img src="../../picture/imagebird.jpg" alt="pic" style="border-radius:50%; width:136px; height:136px" >
                    <div class="caption">Lorem ipsum</div>
                </div>
                <div class="imgborder" style="width: 169.95px; height:136px">
                    <img src="../../picture/imagebird.jpg" alt="pic" style="border-radius:50%; width:136px; height:136px" >
                    <div class="caption">Lorem ipsum</div>
                </div>
                <div class="imgborder" style="width: 169.95px; height:136px">
                    <img src="../../picture/imagebird.jpg" alt="pic" style="border-radius:50%; width:136px; height:136px" >
                    <div class="caption">Lorem ipsum</div>
                </div> -->

                <bird class="box" v-for="item in 8"  :key="item.id"  :caption="item.caption" />

            </div>
        </div>

        <div class="tripbox">
            <div class="triptopic">Trips</div>
            <div class="cardcontainer">
                <card class="box" v-for="item in 16"  :key="item.id"  :caption="item.caption" />
            </div>
            
        </div>

        
    </div>
</template>

<script>
import bird from '../components/bird.vue'
import card from '../components/card.vue'

export default {
    name:'HomePage',
    components: {
        bird,card

    },
    // data () {
    //     return {
    //         // items: 
    //         // [
    //         //     // {
    //         //     //     id:1,
    //         //     //     caption:'Lorem ipsum'
    //         //     // },
    //         //     // {
    //         //     //     id:2,
    //         //     //     caption:'Lorem test'
    //         //     // },
    //         //     // {
    //         //     //     id:3,
    //         //     //     picture:"../../picture/imagebird.jpg",
    //         //     //     caption:'Lorem ipsum'
    //         //     // },
    //         //     // {
    //         //     //     id:4,
    //         //     //     picture:"../../picture/imagebird.jpg",
    //         //     //     caption:'Lorem ipsum'
    //         //     // },
    //         //     // {
    //         //     //     id:5,
    //         //     //     picture:"../../picture/imagebird.jpg",
    //         //     //     caption:'Lorem ipsum'
    //         //     // },
    //         // ]
            
       //}
   // }
}   
</script>

<style>
    
    .home {
        
        width: 100%;
        height: 100%;
    }

    .navbar {
        display:flex;
        
        width: 1440px;
        height: 64px;
        justify-content: space-between;
        background: #FFFFFF;
    }

    .logo {
        display:flex;
        margin-left: 80px;
        width: 82px;
        /* height: 47px; */
        font-family: 'Sarabun';
        font-style: normal;
        font-weight: 700;
        font-size: 36px;
        line-height: 47px;
        align-items: center;
    }
    .menu {
        display:flex;
        width: 394px;
        justify-content: space-between;
        margin-right: 80px;
        align-items: center;
    }

    .trip {
        
        width: 35px;
        height: 23px;

        /* Regular/20 */

        font-family: 'Roboto';
        font-style: normal;
        font-weight: 400;
        font-size: 20px;
        line-height: 23px;

        /* black */

        color: #333333;
    }

    .blog {
        width: 40px;
        height: 23px;

        /* Regular/20 */

        font-family: 'Roboto';
        font-style: normal;
        font-weight: 400;
        font-size: 20px;
        line-height: 23px;
        /* black */
        color: #333333;
    }

    .faq {
        width: 37px;
        height: 23px;
        /* Regular/20 */
        font-family: 'Roboto';
        font-style: normal;
        font-weight: 400;
        font-size: 20px;
        line-height: 23px;
        /* black */
        color: #333333;
    }

    .contact {
        width: 70px;
        height: 23px;
        /* Regular/20 */
        font-family: 'Roboto';
        font-style: normal;
        font-weight: 400;
        font-size: 20px;
        line-height: 23px;
        /* black */
        color: #333333;
    }
    .logingroup {
        width: 100px;
        height: 23px;
        display: flex;
        justify-content: space-between;
    }
    .login {
        width: 60px;
        height: 26px;

        font-family: 'Sarabun';
        font-style: normal;
        font-weight: 400;
        font-size: 20px;
        line-height: 26px;
        /* identical to box height */


        /* Gray 1 */

        color: #333333;
    }

    .rectangle2 {
        display:flex;
        width: 100%;
        height: 733px;
        background: #000000;
        border-inline-start: #000000;
        justify-content: center;
    }

    .tripbox {
        display:flex;
        width: 100%;
        height: 2469px;
        background: #D9D9D9;
    }

    .rectopic {
        position:absolute;
        display:flex;
        width: 445px;
        height: 42px;

        /* Bold/36 */

        font-family: 'Roboto';
        font-style: normal;
        font-weight: 700;
        font-size: 36px;
        line-height: 42px;

        /* white */

        color: #FFFFFF;
        margin-top: 64px;
        margin-bottom: 21px;
    }
    .p1 {
        position:absolute;
        margin-top: 127px;
        width: 737px;
        height: 28px;

/* Regular/24 */

        font-family: 'Roboto';
        font-style: normal;
        font-weight: 400;
        font-size: 24px;
        line-height: 28px;
        text-align: center;

/* white */

        color: #FFFFFF;
    }

    .birdcontainer {
        position:absolute;
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        width: 800px;
        height: 350px;
        margin-top: 244px;
    }
    .item {
        position:absolute;
        display: flex;
        justify-content: center;
    }
    .imgborder {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
    }
    .caption {
        width: 93px;
        height: 19px;

        /* Light/16 */

        font-family: 'Roboto';
        font-style: normal;
        font-weight: 300;
        font-size: 16px;
        line-height: 19px;
        /* identical to box height */

        text-align: center;
        margin-top: 4px;
        /* white */

        color: #FFFFFF;
    }
    .box {
        display:flex;
        flex-wrap: wrap;
    }

    .tripbox {
       display: flex;
       justify-content: center;
    }

    .triptopic {
        margin-top: 52px;
        margin-bottom: 40px;
        position: absolute;
        width: 199px;
        height: 38px;

/* Bold/32 */

        font-family: 'Roboto';
        font-style: normal;
        font-weight: 700;
        font-size: 32px;
        line-height: 38px;
/* identical to box height */

        text-align: center;

        color: #000000;
    }
    .cardcontainer {
        position:absolute;
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        width: 1440px;
        height: 2155px;
        margin-top: 130px;
    }
</style>