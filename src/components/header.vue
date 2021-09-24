<template>
<div>
  <img src="../assets/imgCom/dc-logo.png" alt="logo DC">
  <ul>
    <li v-for= "(link,index) in linkHeader" :key="index">
      <a class="">{{link.text}}</a>
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

<style>

ul{
  list-style: none;
}

</style>