<template>
  <div class="card">
    <div class="imgborder" style="width: 302px; height:524px">
        <div class="cardpic">
            <img src="../../picture/Rectangle.jpg" alt="pic" style=" width:302px; height:378px" >
        </div>

        <div class="cardcaption">
            lorem ipsum
        </div>

        <div class="locationcontainer">
            <img src="../../picture/location.jpg" alt="" style="margin-right:5px;"><div>  location</div>
        </div>

        <div class="price">$ 80</div>

    </div>
   </div>
</template>

<script>
export default {
    name: "CardPic",
    props: {
        picture: {
            type: String,
            default:''
        },
        caption: {
            type: String,
            default:''
        }
    }
}
</script>

<style>
    .price{
        display:flex;
        width:100%;
        height:23px;
        justify-content: end;
        margin-right: 16px
    }

    .locationcontainer {
        display:flex;
        justify-content: start;
        width: 100%;
        height: 23px;
        margin-left: 17px;
    }

    .imgborder {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
    }
    .cardpic {
        display:flex;
        
        width:302px; 
        height:378px;
    }

    .card {
        display:flex;
        flex-wrap: wrap;
        width:302px;
        height: 524px;

        left: 0%;
        right: 0%;
        top: 0%;
        bottom: 0.19%;

        /* white */

        background: #FFFFFF;
        box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.1);
        border-radius: 4px;
        margin-left:12px;
        margin-right:12px;
        margin-bottom: 41px;
    }
    .cardcaption{
        display: flex;

        left: 5.63%;
        right: 55.3%;
        top: 75.81%;
        bottom: 19.81%;

        /* Bold/20 */

        font-family: 'Roboto';
        font-style: normal;
        font-weight: 700;
        font-size: 20px;
        line-height: 23px;
        text-align: center;

        /* black */

        color: #333333;
            width: 100%;
            height: 23px;
            margin-left: 17px;
    }
</style>