<template>
  <div class="LoadingAnimation">
    <div class="LoadingAnimationText">
      Welcome to my world.
    </div>
  </div>
</template>

<style scoped>
  .LoadingAnimation{
    display:flex;
    justify-content:center;
    height:100%;
    background-color:"#939393"
  }
  
  .LoadingAnimationText{
    opacity:0;
    height:100%;
    align-self:center;
    animation: epicFadeInFadeOut 5s;
    font-size:25px;
    color: #dee2e6;
    background-color:black;
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