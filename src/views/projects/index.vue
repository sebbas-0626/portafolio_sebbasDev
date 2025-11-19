<template>
  <div class="projects-index">
    <CardProject :projects="projectsData" :isShow="true"/>
  </div>
</template>
<script setup>
import CardProject from '@/components/CardProject.vue';
import { projectsData } from '@/data/projects.js';
</script>
<style scoped></style>
