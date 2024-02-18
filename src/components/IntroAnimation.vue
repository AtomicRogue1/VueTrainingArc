<template>
  <div class="LoadingAnimation">
    <div class="LoadingAnimationText">
      Welcome to my world.
    </div>
  </div>
</template>

<style scoped>
  .LoadingAnimation{
    bottom:49%;
  }
  
  .LoadingAnimationText{
    opacity:0;
    animation: epicFadeInFadeOut 5s;
    font-size:25px;
    text-align:center;
    color: #3d3b4e;
  }

  @keyframes epicFadeInFadeOut{
    0%{
      opacity:0;
    }
    25%{
      opacity:1;
    }
    75%{
      opacity:1;
    }
    100%{
      opacity:0;
    }
  }
</style>