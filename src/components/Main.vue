<template>
    <div>
        <div class="primaBanda">
            <Fumetti/>
        </div>
        <div class="secondaBanda">
        </div>
        <div class="terzaBanda">
            <div>
                <h5>DC Comics</h5>

            <ul>
                <li v-for= "(link,index) in dcComics" :key="index">
                <a href="#" class="active">{{link.text}}</a>
                </li>
            </ul>

            </div>

            <div>
                <h5>Shop</h5>

            <ul>
                <li v-for= "(link,index) in dcComics" :key="index">
                <a href="#" class="active">{{link.text}}</a>
                </li>
            </ul>

            </div>

            <div>
                <h5>DC</h5>
            <ul>
                <li v-for= "(link,index) in DC" :key="index">
                <a href="#" class="active">{{link.text}}</a>
                </li>
            </ul>

            </div>

            <div>
                <h5>Sites</h5>
            <ul>
                <li v-for= "(link,index) in sites" :key="index">
                <a href="#" class="active">{{link.text}}</a>
                </li>
            </ul>

            </div>

            <img class="logo-bg" src="../assets/imgCom//dc-logo-bg.png" alt="logo-bg">
        </div>

    </div>
</template>

<script>

import Fumetti from "./Fumetti.vue";

export default {
  name:'Fumetti',
  components:{
    Fumetti,
  },
  data:function(){
    return{
      comics:[
        {
        thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
        price: "$19.99",
        series: "Action Comics",
        type: "comic book"
        },

      ]
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

    display: flex;
    
}
.logo-bg{
    height: 400px;
}
h5{
    color: white;
}






</style>