<template>
  <div class="introContainer">
    <div>
      <img class="pfp" src="pfp2.jpg"/>
    </div>
    <div class="introContainerTextItem">
      <p>
      Hi, I'm <span class="imp">Yash Verma</span> and welcome to my portfolio site, made by yours truly! 
      </p>
      <span class="lineBreak"></span>
      <p>My journey in the world of computer science and engineering has been shaped by a combination of education, professional experience, and a relentless curiosity. I am passionate about technology, and I am always eager to learn and grow in this field. I believe that technology can be used to solve complex problems and make the world a better place. I hope you enjoy your time on my site! 
      </p>
    </div>
  </div>
</template>

<style scoped>
  .pfp{
    width:100%;
    border-radius:50%;
  }
  
  .introContainer{
    display:grid;
    grid-column: 2; 
    grid-template-columns: 300px 1fr;
    grid-column-gap:25px;
    padding-bottom:20px;
  }

  .introContainerTextItem{
    display:flex; 
    flex-wrap: wrap;
    justify-items:center;
    align-content:center;
  }

  .imp{
    font-weight:bold;
  }

  /* My version of line break */
  .lineBreak { 
      display: block; 
      margin-bottom: 1em; 
  } 
  
</style>