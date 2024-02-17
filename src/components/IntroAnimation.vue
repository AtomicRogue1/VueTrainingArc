<template>
  <div class="LoadingAnimation">
    <div class="LoadingAnimationText">
      Welcome to my world.
    </div>
  </div>
</template>

<style scoped>
  .LoadingAnimation{
    display:inline-block;
    margin:auto;
    align-self: center;
    justify-self: center;
    background-color:red;
  }
  
  .LoadingAnimationText{
    opacity:0;
    animation: epicFadeInFadeOut 5s;
    font-size:25px;
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