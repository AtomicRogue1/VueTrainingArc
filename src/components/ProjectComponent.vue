<script setup>
  const { name, pic, desc, link } = defineProps(['name', 'pic', 'desc', 'link']);
</script>

<template>
  <div class="projComponent">
    <h3>{{name}}</h3>
    <img v-if="pic!=''" class="projectPic" :src="pic" :alt="name"/>
    <div v-else style="align-content:center" class="defaultProjectPic">
    <img style="width:75px;" src="ProjectPics/project.png" :alt="name"/>
    </div>
    <p style="padding-left:15px; padding-right:15px;">{{desc}}</p>
    <a v-if="link" :href="link">Link to Project</a>
  </div>
</template>



<style scoped>
  .projComponent{
    justify-self:center;
    text-align:center;
    width:100%;
    border-style:solid;
    border-color: #3d3b4e;
    border-width:1px;
    border-radius: 20px 20px 20px 20px;
    padding-bottom:20px;
  }
  .projectPic{
    border-radius:50%;
    width: 100px;
    height: 100px;
  }
  .defaultProjectPic{
    border-radius:50%;
    display:flex;
    justify-content:center;
  }
</style>