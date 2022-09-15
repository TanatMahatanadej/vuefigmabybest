<template>
  <div class="bird">
    <div class="imgborder" style="width: 169.95px; height:136px">
        <div class="birdpic">
            <img src="../../picture/imagebird.jpg" alt="pic" style="border-radius:50%; width:136px; height:136px" >
        </div>

        <div class="caption">
            lorem ipsum
        </div>
    </div>

        
  </div>
</template>

<script>
export default {
    name: "BirdPic",
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
    .imgborder {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
    }

    .birdpic {
        display:flex;
        border-radius:50%; 
        width:136px; 
        height:136px;
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
    .bird {
        display:flex;
        flex-wrap: wrap;
    }
</style>