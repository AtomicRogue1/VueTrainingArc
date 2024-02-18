<template>
  <div>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Open+Sans&display=swap" rel="stylesheet">
    <Intro class="main1" v-if="isLoading"/>
    <div class="ForAnimation main2" v-else>
      <Introduction/>
      <hr style="width:75%;margin-top: 45px;margin-bottom: 45px;"/>
      <Projects/>
      <img class="earth" src="/public/earthSpin.gif"/>
      
    </div>
  </div>
</template>

<script>
  import Intro from './components/IntroAnimation.vue';
  import Introduction from './components/Introduction.vue';
  import Projects from './components/Projects.vue';
  import Socials from './components/FloatingSocials.vue';
  
  export default{
    components:{
      Intro, Introduction, Projects
    },
    data(){
      return{
        isLoading:true,
      };
    },
    mounted(){
      setTimeout(()=>{
        this.isLoading=false;
      },5000);
    }
  }
</script>

<style scoped>
  /* This class is for intro animation alone, due to margin issues.*/
  .main1{     
    color: #dee2e6;
    font-family: 'Open Sans', sans-serif;
  }

  /* Other than intro animation, every component will have this class for sure.*/
  .main2{
    color: #3d3b4e;
    font-family: 'Open Sans', sans-serif;
    align-items:center;
    margin-left:12%;
    margin-right:12%;
    margin-top:12%;
  }

  /* For animating "Welcome to my world." */
  .ForAnimation{
    animation: epicFadeIn 1s;
    animation-iteration-count: 1;
  }

  .earth {
      position: sticky;
      bottom: -100px ;
      left: 50%;
      transform: translateX(-50%) scale(2);
  }

  @keyframes epicFadeIn{
    0%{
      opacity:0;
      margin-top:20%
    }
    100%{
      opacity:1;
      margin-top:12%;
    }
  }
</style>