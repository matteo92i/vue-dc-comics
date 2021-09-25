<template>
    <div>
        <div class="primaBanda">
            <h4>--Content goes here-- </h4>
        </div>
        <div class="secondaBanda">
        </div>
        <div class="terzaBanda"></div>

    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss">
@import "./style/variabili.scss";

.primaBanda{
    height: 100px;
    background-color: $bandacolor;
}
h4{
    font-size: 30px;
    color: $bandacolortext;
    margin-left: 120px;
    line-height: 100px;
}
.secondaBanda{
    height: 150px;
    background-color: $secondaBandaColor;
}
.terzaBanda{
    width: 100%;
    height: 300px;
    background-image: url("../assets/imgCom/jumbotron.jpg");
   
    background-repeat: no-repeat;
    background-size: cover;
}






</style>