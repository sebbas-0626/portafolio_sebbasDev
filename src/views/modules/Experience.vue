<template>
  <section id="experiencia" class="w-full lg:w-[740px] mx-auto py-32">

    <h2 class="text-4xl sm:text-2xl md:text-4xl font-semibold mb-6 flex gap-x-3 items-center text-black/80 dark:text-white/80 px-4 md:px-0 transition hover:scale-110">
  <Briefcase class="size-16" />
  <span>Experiencia laboral</span>
</h2>

    <div  class="flex justify-center">
      <ol class="relative border-s border-gray-200 dark:border-gray-700">

        <!-- Información para el proyecto de Turismo Rivera -->

        <li v-for="(experienceItem, index) in experience" :key="index" class="mb-10 ms-4">
          <div class="absolute w-3 h-3 bg-gray-200 rounded-full mt-1.5 -start-1.5 border border-white dark:border-gray-900 dark:bg-gray-700"></div>
          <time class="mb-1 text-sm font-normal leading-none text-gray-400 dark:text-gray-500">{{ experienceItem.company }}</time> <br>
          <time class="mb-1 text-sm font-normal leading-none text-gray-400 dark:text-gray-500">{{ experienceItem.title }} - {{ experienceItem.period }}</time>
          <h3 class="text-lg font-semibold text-gray-900 dark:text-white">{{ experienceItem.proyecto }}</h3>
          <p class="text-base font-normal text-gray-500 dark:text-gray-400">
            {{ experienceItem.description }}
            <a :href="experienceItem.source" class="text-blue-700 hover:underline" target="_blank" rel="noopener noreferrer">Saber más</a>.
          </p>
        </li>
      </ol>
    </div>
  </section>
</template>

<script setup>
import Briefcase from "@/components/icons/Briefcase.vue";
import { experience } from "@/data/experience.js";
</script>

<style scoped>
/* Puedes agregar estilos específicos del componente aquí si es necesario */
</style>
