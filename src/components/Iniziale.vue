<template>
<div class="disposizione">
  <img class="center" src="../assets/imgCom/dc-logo.png" alt="logo DC">
  <ul class="disposizione-ul">
    <li class="disposizione-lista" v-for= "(link,index) in linkHeader" :key="index">
      <a href="#" class="active">{{link.text}}</a>
    </li>
  </ul>

</div>
</template>
  


<script>
export default {
  name:'Iniziale',
  data: function (){
    return {
      linkHeader: [
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
      ]
    }
  }
    
}
</script>

<style Lang="scss">
@import "./style/variabili.scss";

.disposizione{
  height: 90px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.center{
  height: 80px;
  margin-left: 150px;
}
  
.disposizione-ul{
  list-style: none;
  margin-right: 150px;
}

.disposizione-lista{
  float: left;
  font-size: 25px;
  margin-left: 15px;
}
  
a{
  text-decoration: none;
  
}
li a:hover {
  color: blue;
}


  




  


</style>