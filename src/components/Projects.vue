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

<script>
  import ProjectComponent from './ProjectComponent.vue';
  const myprojects = [
    {
      name:"a",
      pic:"./pfp2.jpg",
      desc:"b",
      link:"www.google.com"
    },
    {
      name:"b",
      pic:"./pfp2.jpg",
      desc:"b",
      link:"www.google.com"
    },
    {
      name:"c",
      pic:"./pfp2.jpg",
      desc:"b",
      link:"www.google.com"
    }
  ]
</script>

<style scoped>
  
</style>