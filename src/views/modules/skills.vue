<template>
  <div class="overflow-hidden mx-4 my-12 sm:mx-8 md:mx-16 lg:mx-32">
    <!-- <div
      class="text-2xl sm:text-3xl md:text-4xl font-semibold mb-4 sm:mb-6 flex gap-x-2 sm:gap-x-3 items-center text-black/80 dark:text-white transition hover:scale-110 pl-72 sm:pl-12 md:pl-16">
      <Briefcase class="size-10 sm:size-12 md:size-16" />
      <h2>Skills</h2>
    </div> -->
    <div class="marquee">
      <div class="marquee-content">
        <div v-for="(skill, id) in skillsData" :key="id"
          class="w-28 sm:w-32 md:w-36 min-w-fit h-fit inline-block transition-all duration-500 m-2 sm:m-3 md:m-5 rounded-lg group relative cursor-pointer hover:scale-110">
          <div
            class="h-full w-full rounded-lg border border-gray-400 bg-white dark:bg-black shadow-lg group-hover:border-slate-400 group-hover:shadow-slate-600 transition-all duration-500">
            <div class="flex -translate-y-[1px] justify-center">
              <div class="w-3/4">
                <div class="h-[1px] w-full bg-gradient-to-r from-transparent via-neutral-600 to-transparent" />
              </div>
            </div>

            <div class="flex flex-col items-center justify-center gap-2 sm:gap-3 p-3 sm:p-4 md:p-6">
              <div class="h-6 sm:h-8 md:h-10">
                <img :src="skill.icon" :alt="skill.name" width="40" height="40"
                  class="h-full w-auto rounded-lg" />
              </div>
              <p class="text-black/80 dark:text-white/80 text-xs sm:text-sm md:text-lg">
                {{ skill.name }}
              </p>
            </div>
          </div>
        </div>
      </div>
      <!-- Duplicado para efecto infinito -->
      <div class="marquee-content" aria-hidden="true">
        <div v-for="(skill, id) in skillsData" :key="`duplicate-${id}`"
          class="w-28 sm:w-32 md:w-36 min-w-fit h-fit inline-block transition-all duration-500 m-2 sm:m-3 md:m-5 rounded-lg group relative cursor-pointer hover:scale-110">
          <div
            class="h-full w-full rounded-lg border border-gray-700 bg-gray-900 shadow-lg group-hover:border-violet-500 group-hover:shadow-violet-500/50 transition-all duration-500">
            <div class="flex -translate-y-[1px] justify-center">
              <div class="w-3/4">
                <div class="h-[1px] w-full bg-gradient-to-r from-transparent via-violet-500 to-transparent" />
              </div>
            </div>

            <div class="flex flex-col items-center justify-center gap-2 sm:gap-3 p-3 sm:p-4 md:p-6">
              <div class="h-6 sm:h-8 md:h-10">
                <img :src="skill.icon" :alt="skill.name" width="40" height="40"
                  class="h-full w-auto rounded-lg" />
              </div>
              <p class="text-white text-xs sm:text-sm md:text-lg">
                {{ skill.name }}
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { skillsData } from "@/data/skills";
import Briefcase from "@/components/icons/Briefcase.vue";

</script>

<style scoped>
.marquee {
  display: flex;
  width: 100%;
  user-select: none;
}

.marquee:hover .marquee-content {
  animation-play-state: paused;
}

.marquee-content {
  display: flex;
  animation: scroll 30s linear infinite;
  white-space: nowrap;
}

@keyframes scroll {
  0% {
    transform: translateX(0);
  }

  100% {
    transform: translateX(-50%);
  }
}
</style>
