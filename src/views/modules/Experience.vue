<template>
  <section id="experiencia" class="w-full lg:w-[740px] mx-auto py-32">

    <h2 class="text-4xl sm:text-2xl md:text-4xl font-semibold mb-6 flex gap-x-3 items-center text-black/80 dark:text-white/80 px-4 md:px-0 transition hover:scale-110">
  <Briefcase class="size-16" />
  <span>Experiencia laboral</span>
</h2>

    <div class="flex justify-center">
      <ol class="relative border-s border-gray-200 dark:border-gray-700">

        <!-- Información para el proyecto de Turismo Rivera -->

        <li class="mb-10 ms-4">
          <div class="absolute w-3 h-3 bg-gray-200 rounded-full mt-1.5 -start-1.5 border border-white dark:border-gray-900 dark:bg-gray-700"></div>
          <time class="mb-1 text-sm font-normal leading-none text-gray-400 dark:text-gray-500">Enero 2024 - En proceso</time>
          <h3 class="text-lg font-semibold text-gray-900 dark:text-white">Proyecto Turismo Rivera</h3>
          <p class="text-base font-normal text-gray-500 dark:text-gray-400">
            Contribuidor en el desarrollo la pagina web de turismo para el pueblo de Rivera, Huila. Puedes seguir el progreso en
            <a href="https://github.com/oscarruiz05/turismo-rivera-web" class="text-blue-700 hover:underline" target="_blank" rel="noopener noreferrer">GitHub</a>.
          </p>
        </li>

        <!-- Información para el trabajo como desarrollador frontend en Cootranshuila LTDA -->
        <li class="mb-10 ms-4">
          <div class="absolute w-3 h-3 bg-gray-200 rounded-full mt-1.5 -start-1.5 border border-white dark:border-gray-900 dark:bg-gray-700"></div>
          <time class="mb-1 text-sm font-normal leading-none text-gray-400 dark:text-gray-500">Septiembre 2023 - En proceso</time>
          <h3 class="text-lg font-semibold text-gray-900 dark:text-white"> Frontend en Cootranshuila LTDA</h3>
          <p class="text-base font-normal text-gray-500 dark:text-gray-400">
            Contribuí  como desarrollo de la pagina web  actual de la empresa Cootranshuila LTDA. Puedes revisar el código en
            <a href="https://github.com/Cootranshuila-LTDA/cootranshuila-web-front" class="text-blue-700 hover:underline" target="_blank" rel="noopener noreferrer">GitHub</a>.
          </p>
        </li>

        <!-- Información para el trabajo en el backend de Cootranshuila LTDA -->
        <li class="mb-10 ms-4">
          <div class="absolute w-3 h-3 bg-gray-200 rounded-full mt-1.5 -start-1.5 border border-white dark:border-gray-900 dark:bg-gray-700"></div>
          <time class="mb-1 text-sm font-normal leading-none text-gray-400 dark:text-gray-500">Septiembre 2023 - En proceso</time>
          <h3 class="text-lg font-semibold text-gray-900 dark:text-white"> Backend de Cootranshuila LTDA</h3>
          <p class="text-base font-normal text-gray-500 dark:text-gray-400">
            Contribuí en la diagramación y desarrollo del backend para el proyecto de Cootranshuila LTDA. Puedes revisar el código en
            <a href="https://github.com/Cootranshuila-LTDA/cootranshuila-web-back" class="text-blue-700 hover:underline" target="_blank" rel="noopener noreferrer">GitHub</a>.
          </p>
        </li>

        <!-- Información para los proyectos de WordPress -->
        <li class="mb-10 ms-4">
          <div class="absolute w-3 h-3 bg-gray-200 rounded-full mt-1.5 -start-1.5 border border-white dark:border-gray-900 dark:bg-gray-700"></div>
          <time class="mb-1 text-sm font-normal leading-none text-gray-400 dark:text-gray-500">Mayo 2023 - Septiembre</time>
          <h3 class="text-lg font-semibold text-gray-900 dark:text-white">Proyectos de WordPress</h3>
          <p class="mb-4 text-base font-normal text-gray-500 dark:text-gray-400">
            Desarrollé y completé dos proyectos en WordPress utilizando Divi y Elementor. Puedes ver los proyectos en
            <a href="https://clinicahispanairvingtx.com/medicina-familiar/" class="text-blue-700 hover:underline" target="_blank" rel="noopener noreferrer">Clínica Hispana</a> (Divi) y
            <a href="https://riverahuila.com/" class="text-blue-700 hover:underline" target="_blank" rel="noopener noreferrer">Turismo Rivera</a> (Elementor).
          </p>
        </li>


        <!-- Información para el trabajo como desarrollador en el sistema de inventario -->
        <li class="mb-10 ms-4">
          <div class="absolute w-3 h-3 bg-gray-200 rounded-full mt-1.5 -start-1.5 border border-white dark:border-gray-900 dark:bg-gray-700"></div>
          <time class="mb-1 text-sm font-normal leading-none text-gray-400 dark:text-gray-500">Mayo 2023 - julio 2023</time>
          <h3 class="text-lg font-semibold text-gray-900 dark:text-white">Sistema de inventario</h3>
          <p class="mb-4 text-base font-normal text-gray-500 dark:text-gray-400">
            Contribuí en el desarrollo del sistema de inventario para una panaderia en Laravel 9 y Vue 3. Puedes encontrar el proyecto en
            <a href="https://github.com/oscarruiz05/inventario" class="text-blue-700 hover:underline" target="_blank" rel="noopener noreferrer">GitHub</a>.
          </p>
        </li>
      </ol>
    </div>
  </section>
</template>

<script>
import Briefcase from "@/components/icons/Briefcase.vue";
export default {
  components: { Briefcase },
};
</script>

<style scoped>
/* Puedes agregar estilos específicos del componente aquí si es necesario */
</style>
