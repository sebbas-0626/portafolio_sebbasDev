<template>
  <header
    class="font-sans flex items-center mx-auto py-10 sticky top-0 w-full md:w-[1120px] z-10  text-black/80 dark:text-white/80">
    <nav
      class="border border-white w-full rounded-full px-4 py-2 flex flex-row justify-center md:justify-between backdrop-blur-2xl shadow-md">
      <div id="logo" class="h-16 hidden md:flex items-center max-w-48 font-bold text-2xl mx-5">
        <a href="/#">
          <!-- <span class="text-slate-600 dark:text-white">
            Sebastian <br class="text-sm" />developer</span -->
          <div class="translate-x-4 transition duration-1000 ease-in-out">
            <CodeVue class="size-16" />
          </div>
        </a>
      </div>
      <div id="nav" class="flex gap-3 justify-between items-center text-black dark:text-white text-xs md:text-base">
        <LightDark />

        <a href="#experiencia" class="nav-link hover:bg-white/10 rounded-full px-3 transition">Experience</a>
        <router-link to="/projects"
          class="nav-link hover:bg-white/10 rounded-full px-3 transition">Projects</router-link>
        <a href="#about-me" class="nav-link hover:bg-white/10 rounded-full px-3 transition">sobre me</a>


      </div>
    </nav>
  </header>
</template>

<script>
import LightDark from "./icons/Light&Dark.vue";
import CodeVue from "./icons/Code.vue";
export default {
  components: { LightDark, CodeVue },
  mounted() {
    // Manejar clic en enlaces de navegación (solo para anclas #)
    const navLinks = document.querySelectorAll('a.nav-link[href^="#"]');
    navLinks.forEach(link => {
      link.addEventListener('click', this.scrollToSection);
    });
  },
  methods: {
    scrollToSection(event) {
      event.preventDefault();
      const targetId = event.currentTarget.getAttribute('href').substring(1);
      const targetElement = document.getElementById(targetId);

      if (targetElement) {
        targetElement.scrollIntoView({ behavior: 'smooth' });
      }
    }
  }
};
</script>

<style></style>
