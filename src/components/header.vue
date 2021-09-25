<template>
<div class="disposizione">
  <img src="../assets/imgCom/dc-logo.png" alt="logo DC">
  <ul>
    <li v-for= "(link,index) in linkHeader" :key="index">
      <a href="#" :class="active">{{link.text}}</a>
    </li>
  </ul>

</div>
</template>
  


<script>
export default {
  name:'Header',
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
  height: 100px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
  
ul{
  list-style: none;
}

li{
  float: left;
  margin: 15px 15px;
}
a{
  text-decoration: none;
  
}
li a:hover {
  color: blue;
}


  




  


</style>