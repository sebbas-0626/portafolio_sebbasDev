<template>
  <main>
    <section class="w-full lg:w-[740px] mx-auto py-12 md:py-20 lg:py-20 text-center">
      <div class="px-28">
        <img class="rounded-full size-20 mb-4" src="/img/sebas.jpg" alt="SebbasDEV logo" />
      </div>
      <h1
        class="text-black dark:text-white text-3xl md:text-4xl lg:text-5xl font-bold flex justify-center flex-row mb-4 transition hover:scale-110">
        <span class="text-blue-600">Hey</span>, soy Sebastian
      </h1>
      <div class="flex justify-center items-center py-6">
        <BadgeVue>Disponible para trabajar</BadgeVue>
      </div>
      <h2 class="text-black dark:text-white text-sm md:text-base lg:text-lg">
        🚀 Desarrollador Web. De Colombia, <span class="text-blue-600 font-bold">con experiencia en proyectos </span>
        colaborativos en empresas,
        <span class="text-blue-600 font-bold">
          aportando en el desarrollo
        </span>
        tanto en el frontend como en el
        <span class="text-blue-600 font-bold"> backend. </span>
        Mi experiencia diaria me ha permitido entender
        <span class="text-blue-600 font-bold"> la importancia del </span>

        trabajo constante y dedicado.
        <span class="text-blue-600 font-bold">
          Descubre más sobre mis contribuciones
        </span>
        en mis
        <span class="text-blue-600 font-bold"> repositorios de GitHub,</span>
        donde reflejo mi pasión y habilidades técnicas. 💻✨
      </h2>
      <nav class="flex gap-4 mt-8 flex-wrap justify-center">
        <SocialPillVue href="/src/assets/cv/Dev-SebastianTovarChavez.pdf" download>
          <Cv class="size-4 md:size-6"></Cv>
          Descargar CV
        </SocialPillVue>
        <SocialPillVue href="https://github.com/sebbas-0626">
          <GitHub class="size-4 md:size-6"></GitHub>
          GitHub
        </SocialPillVue>

        <SocialPillVue href="https://www.linkedin.com/in/sebbasdev/">
          <LinkedInVue class="size-4 md:size-6"></LinkedInVue>
          LinkedIn
        </SocialPillVue>

        <SocialPillVue href="mailto:sebastiantovarchavez304@gmail.com">
          <MailVue class="size-4 md:size-6"></MailVue>
          sebastiantovarchavez304@gmail.com
        </SocialPillVue>
      </nav>
    </section>
  </main>
</template>

<script>
import BadgeVue from "@/components/icons/Badge.vue";
import Cv from "@/components/icons/Cv.vue";
import GitHub from "@/components/icons/GitHub.vue";
import LinkedInVue from "@/components/icons/LinkedIn.vue";
import MailVue from "@/components/icons/Mail.vue";
import SocialPillVue from "@/components/icons/SocialPill.vue";
export default {
  components: { BadgeVue, Cv, GitHub, SocialPillVue, MailVue, LinkedInVue },
};
</script>

<style></style>
