<template>
  <footer class="rounded-lg shadow m-4 bg-black/5 dark:bg-black/20 backdrop-blur-lg w-full xl:w-[1120px] mx-auto mb-10">
    <div class="w-full mx-auto max-w-screen-xl p-4 md:flex md:items-center md:justify-between">
      <div class="flex flex-col items-center md:flex-row md:items-center md:justify-between w-full text-center md:text-left">
        <span class="text-sm font-bold text-black dark:text-white mb-4 md:mb-0 md:mr-6">
          © {{ year }} <a href="https://sebbasdev0626.netlify.app/" class="hover:underline">SebbasDEV</a>. Diseño basado en  una iniciativa de midudev
        </span>
        <ul class="flex flex-wrap items-center justify-center mt-3 text-sm font-medium dark:text-white/90 sm:mt-0 md:justify-end">
          <li>
            <a href="/#" class="hover:underline me-4 md:me-6 font-bold">Home</a>
          </li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<script setup>
const year = '2025';
</script>

<style scoped>
</style>
