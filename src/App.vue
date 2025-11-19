<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HeaderVue from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";
import "@fontsource/open-sans/700.css" ;


</script>

<template>
  <HeaderVue />
  <RouterView />
  <Footer />
</template>

<style scoped></style>
