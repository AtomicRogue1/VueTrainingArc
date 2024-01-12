<template>
  <div style="padding-bottom:20px;">
    <h2>Projects</h2>
    <div class="projects">
      <ProjectComponent v-for="project in myprojects"
      :name="project.name"
      :pic="project.pic"
      :desc="project.desc"
      :link="project.link"
      :key="project.name"
      />
    </div>
  </div>
</template>

<script setup>
  import ProjectComponent from './ProjectComponent.vue';
  const myprojects = [
    {
      name:"The Lighthouse (Game)",
      pic:"ProjectPics/Lighthouse.png",
      desc:"2D platformer game, where I added more game mechanics to add more ways to play and made an experimental Cinematic system.",
      link:"https://github.com/AtomicRogue1/ProjectLighthouse"
    },
    {
      name:"Blockchain Contact Tracing App",
      pic:"pfp.jpg",
      desc:"Frontend made for blockchain contact tracing app that does COVID contact tracing with help of anonymity offered by blockchain.",
      link:"https://github.com/Blockhain-Contact-Tracing/new-frontend"
    },
    {
      name:"Queue Management System",
      pic:"./pfp.jpg",
      desc:"Queue management system made using HTML, CSS, Python for backend and Twilio.",
    },
    {
      name:"CamScribbler",
      pic:"./pfp.jpg",
      desc:"Software made as an alternative for use of graphic tablets. Uses YOLO CV framework to draw on the digital canvas."
    },
    {
      name:"Ancient Helm Program",
      pic:"./ProjectPics/project.png",
      desc:"AR swordfight simulator made as a tribute to Legend of Zelda: Breath of the Wild. Work in progress."
    }
  ]
</script>

<style scoped>
  .projects{
    display:grid;
    grid-template-columns:1fr 1fr 1fr;
    grid-gap:25px;
  }
</style>