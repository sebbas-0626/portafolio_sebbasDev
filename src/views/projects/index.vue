<template>
  <div class="projects-index">
    <!-- <Projects /> -->
    <CardProject :projects="projectsData" :isShow="true"/>
  </div>
</template>
<script setup>
import Projects from '@/views/modules/Projects.vue';
import CardProject from '@/components/CardProject.vue';
import { projectsData } from '@/data/projects.js';
</script>
<style scoped></style>
