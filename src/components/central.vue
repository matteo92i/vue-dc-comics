<template>
    <div>
        <div class="primaBanda">
            <h4>--Content goes here-- </h4>
        </div>
        <div class="secondaBanda">
        </div>
        <div class="terzaBanda">
            <ul>
                <li v-for= "(link,index) in dcComics" :key="index">
                <a href="#" class="active">{{link.text}}</a>
                </li>
            </ul>
            <img class="logo-bg" src="../assets/imgCom//dc-logo-bg.png" alt="logo-bg">
        </div>

    </div>
</template>

<script>
export default {
     name:'central',
  data: function (){
    return {
      dcComics: [
        {
          text:'charater',
          link: '#charater',
        },
        {
          text:'comics',
          link: '#comics',
        },
                {
          text:'movies',
          link: '#movies',
        },
        {
          text:'tv',
          link: '#tv',
        },
                {
          text:'games',
          link: '#games',
        },
        {
          text:'collections',
          link: '#collections',
        },
                {
          text:'video',
          link: '#video',
        },
        {
          text:'fans',
          link: '#fans',
        },
                {
          text:'news',
          link: '#news',
        },
        {
          text:'shop',
          link: '#shop',
        },
      ],
      shop:[
          {
              text:'shop',
              link: '#shop',
          },
          {
              text:'shop',
              link: '#shop',
          }
      ],
    DC: [
        {
          text:'charater',
          link: '#charater',
        },
        {
          text:'comics',
          link: '#comics',
        },
                {
          text:'movies',
          link: '#movies',
        },
        {
          text:'tv',
          link: '#tv',
        },
                {
          text:'games',
          link: '#games',
        },
        {
          text:'collections',
          link: '#collections',
        },
                {
          text:'video',
          link: '#video',
        },
        {
          text:'fans',
          link: '#fans',
        },
                {
          text:'news',
          link: '#news',
        },
        {
          text:'shop',
          link: '#shop',
        },
      ],
    sites: [
        {
          text:'charater',
          link: '#charater',
        },
        {
          text:'comics',
          link: '#comics',
        },
                {
          text:'movies',
          link: '#movies',
        },
        {
          text:'tv',
          link: '#tv',
        },
                {
          text:'games',
          link: '#games',
        },
        {
          text:'collections',
          link: '#collections',
        },
                {
          text:'video',
          link: '#video',
        },
        {
          text:'fans',
          link: '#fans',
        },
                {
          text:'news',
          link: '#news',
        },
        {
          text:'shop',
          link: '#shop',
        },
      ],

    }
  }
    
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
    height: 400px;
    background-image: url("../assets/imgCom/footer-bg.jpg");
   
    background-repeat: no-repeat;
    background-size: cover;
}
.logo-bg{
    height: 400px;
}






</style>