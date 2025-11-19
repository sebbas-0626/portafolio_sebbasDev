<script setup>
import Info from "@/views/modules/info.vue";
import CardProject from "@/components/CardProject.vue";
import { projectsData } from "@/data/projects.js";
import Experience from "@/views/modules/Experience.vue";
import Skills from "@/views/modules/skills.vue";
import AboutMe from "./modules/AboutMe.vue";

const homeProjects = projectsData.slice(0, 3);
</script>

<template>
  <Info />
  <Skills />
  <Experience/>
  <CardProject :projects="homeProjects" :isShow="true"/>
  <AboutMe />
</template>
