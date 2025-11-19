<template>
  <div class="w-full py-12 px-4 sm:px-6 lg:px-8">
    <div class="max-w-7xl mx-auto">
      <h2
        class="text-4xl sm:text-2xl md:text-4xl font-semibold mb-6 flex gap-x-3 items-center text-black/80 dark:text-white/80 px-4 md:px-0 transition hover:scale-110">
        <Briefcase class="size-16" />
        <router-link to="/projects">Proyectos</router-link>
      </h2>
      <!-- Grid responsivo para las tarjetas -->
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
        <!-- Card de proyecto -->
        <div v-for="(project, index) in projects" :key="index"
          class="relative flex flex-col rounded-xl bg-white bg-clip-border text-gray-700 shadow-lg hover:shadow-xl transition-shadow duration-300">
          <!-- Imagen del proyecto -->
          <div class="relative overflow-hidden rounded-t-xl bg-gray-200 h-48 sm:h-56">
            <img :src="project.image" :alt="project.title"
              class="w-full h-full object-cover hover:scale-105 transition-transform duration-300" />
            <div class="absolute inset-0 bg-gradient-to-tr from-transparent via-transparent to-black/60"></div>
          </div>
          <!-- Contenido de la tarjeta -->
          <div class="flex flex-col flex-grow p-6">
            <h5 class="text-xl font-semibold text-gray-900 mb-3 line-clamp-2">
              {{ project.title }}
            </h5>

            <p class="text-sm text-gray-600 leading-relaxed mb-4 line-clamp-3 flex-grow">
              {{ project.description }}
            </p>

            <!-- Tags/Tecnologías -->
            <div class="flex flex-wrap items-center gap-2 mb-4">
              <span v-for="(tag, tagIndex) in project.tags" :key="tagIndex"
                class="flex items-center justify-center rounded-full border border-gray-200 bg-gray-50 p-2 hover:bg-gray-100 transition-colors duration-200"
                :title="tag.name || tag">
                <!-- Si el tag es un objeto con icon, mostrar imagen -->
                <img v-if="tag.icon" :src="tag.icon" :alt="tag.name" class="w-6 h-6" />
                <!-- Si el tag es un string, mostrar texto -->
                <span v-else class="text-xs font-medium px-2">{{ tag }}</span>
              </span>
            </div>

            <!-- Botón -->
            <a :href="project.source" target="_blank" rel="noopener noreferrer"
              class="w-full rounded-lg bg-gray-900 py-3 px-6 text-center text-sm font-bold uppercase text-white shadow-md hover:shadow-lg hover:bg-gray-800 transition-all duration-200">
              Ver Código
            </a>
          </div>
        </div>
      </div>
      <!-- boton ver todos los proyectos -->
      <div v-if="isShow" class="flex justify-center mt-8">
        <router-link to="/projects"
          class="inline-block rounded-lg bg-blue-600 py-3 px-6 text-center text-sm font-bold uppercase text-white shadow-md hover:shadow-lg hover:bg-blue-500 transition-all duration-200">
          Ver Todos los Proyectos
        </router-link>
      </div>
    </div>
    </div>


</template>


<script setup>
import Briefcase from "@/components/icons/Briefcase.vue";

// Definir las props que recibe el componente
const props = defineProps({
  projects: {
    type: Array,
    required: true
  },
  isShow: {
    type: Boolean,
    default: false
  }
})
</script>
