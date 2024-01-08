<script setup>
  const { name, pic, desc, link } = defineProps([name,pic,desc,link]);
</script>

<template>
  <div class="projComponent">
    <h3>{{name}}</h3>
    <img :src="pic" :alt="name"/>
    <p>{{desc}}</p>
    <a :href="link">{{link}}</a>
  </div>
</template>



<style scoped>
  .projComponent{
    background-color: #dee2e6;
  }
</style>