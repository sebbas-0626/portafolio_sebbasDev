<template>
  <header
    class="font-sans flex items-center mx-auto py-10 sticky top-0 w-full md:w-[1120px] z-10  text-black/80 dark:text-white/80">
    <nav
      class="border border-white w-full rounded-full px-4 py-2 flex flex-row justify-center md:justify-between backdrop-blur-2xl shadow-md">
      <div id="logo" class="h-16 hidden md:flex items-center max-w-48 font-bold text-2xl mx-5">
        <router-link to="/">
          <div class="translate-x-4 transition duration-1000 ease-in-out">
            <CodeVue class="size-16" />
          </div>
        </router-link>
      </div>
      <div id="nav" class="flex gap-3 justify-between items-center text-black dark:text-white text-xs md:text-base">
        <LightDark />

        <router-link to="/#experiencia" class="nav-link hover:bg-white/10 rounded-full px-3 transition">Experience</router-link>
        <router-link to="/projects"
          class="nav-link hover:bg-white/10 rounded-full px-3 transition">Projects</router-link>
        <router-link to="/#about-me" class="nav-link hover:bg-white/10 rounded-full px-3 transition">sobre me</router-link>


      </div>
    </nav>
  </header>
</template>

<script setup>
import LightDark from "./icons/Light&Dark.vue";
import CodeVue from "./icons/Code.vue";
import { useRouter, useRoute } from 'vue-router';
import { onMounted } from 'vue';

const router = useRouter();
const route = useRoute();

const handleNavClick = (event) => {
  const href = event.currentTarget.getAttribute('href');

  // Si el href contiene un hash
  if (href && href.includes('#')) {
    const hash = href.split('#')[1];

    // Si ya estamos en home, solo hacer scroll
    if (route.path === '/') {
      event.preventDefault();
      const targetElement = document.getElementById(hash);
      if (targetElement) {
        targetElement.scrollIntoView({ behavior: 'smooth' });
      }
    } else {
      // Si estamos en otra página, navegar a home y luego hacer scroll
      event.preventDefault();
      router.push('/').then(() => {
        setTimeout(() => {
          const targetElement = document.getElementById(hash);
          if (targetElement) {
            targetElement.scrollIntoView({ behavior: 'smooth' });
          }
        }, 100);
      });
    }
  }
};

onMounted(() => {
  // Manejar clic en enlaces de navegación con router-link
  const navLinks = document.querySelectorAll('a.nav-link[href*="#"]');
  navLinks.forEach(link => {
    link.addEventListener('click', handleNavClick);
  });
});
</script>

<style></style>
