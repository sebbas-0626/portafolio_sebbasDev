<template>
  <section id="projects" class="w-full lg:w-[740px] mx-auto py-26">
    <h2
      class="text-4xl sm:text-2xl md:text-4xl font-semibold mb-6 flex gap-x-3 items-center text-black/80 dark:text-white/80 px-4 md:px-0 transition hover:scale-110">
      <Code class="size-16" />
      <span>Proyectos</span>
    </h2>


    <div class="flex flex-wrap justify-center gap-8">
      <div class="card"><img src="/img/rivera-huilaWeb.png" alt="" class="h-48">
        <div class="card__content">
          <p class="card__title">Rivera Huila Web</p>
          <ul class="flex gap-x-2 flex-row mb-2">
            <li>
              <span
                class="flex gap-x-2 rounded-full text-xs bg-slate-300 text-black py-1 px-2 items-center border-2 border-solid border-dark">
                <IconAstroVue />
                Astro
              </span>
            </li>
          </ul>
          <p class="card__description"> <span class="text-slate-800">Pagina web rivera turismo </span></p>
          <a href="https://turismo-rivera.vercel.app/" target="_blank" class="bg-slate-300 text-black
      border border-gray-300
      rounded-full
      inline-flex justify-center items-center gap-x-2
      mt-2
      py-1 px-2 md:py-1 md:px-4
      text-xs
      transition
      hover:scale-110 hover:bg-white/10">Ir al sitio web</a>
        </div>
      </div>
      <!-- 2 -->
      <div class="card"><img src="/img/sitema_inventario.png" alt="" class="h-48">
        <div class="card__content">
          <p class="card__title">Sistema de inventario</p>
          <ul class="flex gap-x-2 flex-row mb-2">
            <li><span
                class="flex gap-x-2 rounded-full text-xs bg-white text-dark py-1 px-2 items-center border-2 border-solid border-dark bg-slate-300">
                <IconLaravel />
                Laravel
              </span></li>
            <li><span
                class="flex gap-x-2 rounded-full text-xs bg-white text-dark py-1 px-2 items-center border-2 border-solid border-dark bg-slate-300">
                <IconVueVue />
                Vue js
              </span></li>
          </ul>
          <p class="card__description">Sistema de Invenatrio para una panaderia</p><a
            href="https://github.com/oscarruiz05/inventario" target="_blank" class="bg-white/5
      border border-gray-300 text-black
      rounded-full
      inline-flex justify-center items-center gap-x-2
      mt-2
      py-1 px-2 md:py-1 md:px-4
      text-xs
      transition
      hover:scale-110 hover:bg-white/10 bg-slate-300">Ir al sitio web</a>
        </div>
      </div>
      <!-- 3 -->
      <div class="card"><img src="/img/cootranshuila.png" alt="">
        <div class="card__content">
          <p class="card__title">
            Pagina web cootranshuila
          </p>
          <ul class="flex gap-x-2 flex-row mb-2">
            <li><span
                class="flex gap-x-2 rounded-full text-xs bg-white text-dark py-1 px-2 items-center border-2 border-solid border-dark bg-slate-300">
                <IconVueVue />
                Vue js
              </span></li>
          </ul>
          <p class="card__description">Pagina web para venta de pasajes en linea, con pasarela de pagos incluida</p><a
            href="https://cootranshuila.com/" target="_blank" class="bg-white/5
      border border-gray-300
      rounded-full
      inline-flex justify-center items-center gap-x-2
      mt-2
      py-1 px-2 md:py-1 md:px-4
      text-xs
      transition
      hover:scale-110 hover:bg-white/10 bg-slate-300">Ir al sitio web</a>
        </div>
      </div>

      <!-- four -->
      <div class="card"><img src="/img/hermes.png" alt="">
        <div class="card__content">
          <p class="card__title">Backend Cootranshuila ltda</p>
          <ul class="flex gap-x-2 flex-row mb-2">
            <li><span
                class="flex gap-x-2 rounded-full text-xs bg-white text-dark py-1 px-2 items-center border-2 border-solid border-dark bg-slate-300">
                <IconLaravel />Laravel
              </span></li>

          </ul>
          <p class="card__description">backend de la pagina web cootranshuila</p><a
            href="https://github.com/Cootranshuila-LTDA/cootranshuila-web-back" target="_blank" class="bg-white/5
      border border-gray-300
      rounded-full
      inline-flex justify-center items-center gap-x-2
      mt-2
      py-1 px-2 md:py-1 md:px-4
      text-xs
      transition
      hover:scale-110 hover:bg-white/10 bg-slate-300">Ir al sitio web</a>
        </div>
      </div>


    </div>
  </section>
</template>

<script>
import Code from '@/components/icons/Code.vue';
import IconLaravel from '@/components/iconsCardsProjects/IconLaravel.vue';
import SocialPillVue from '@/components/icons/SocialPill.vue';
import IconAstroVue from '@/components/iconsCardsProjects/IconAstro.vue';
import IconVueVue from '@/components/iconsCardsProjects/IconVue.vue';
export default {
  components: {
    Code,
    SocialPillVue,
    IconLaravel,
    IconAstroVue,
    IconVueVue
  }
};
</script>

<style>
.card {
  position: relative;
  width: 350px;
  aspect-ratio: 16/9;
  background-color: #f2f2f2;
  border-radius: 10px;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  perspective: 1000px;
  box-shadow: 0 0 0 5px #ffffff80;
  transition: all 0.6s cubic-bezier(0.175, 0.885, 0.32, 1.275);
}

.card svg {
  width: 48px;
  fill: #333;
  transition: all 0.6s cubic-bezier(0.175, 0.885, 0.32, 1.275);
}

.card__image {
  width: 100%;
  height: 100%;
}

.card:hover {
  transform: scale(1.05);
  box-shadow: 0 8px 16px rgba(255, 255, 255, 0.2);
}

.card__content {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  padding: 20px;
  box-sizing: border-box;
  background-color: #f2f2f2;
  transform: rotateX(-90deg);
  transform-origin: bottom;
  transition: all 0.6s cubic-bezier(0.175, 0.885, 0.32, 1.275);
}

.card:hover .card__content {
  transform: rotateX(0deg);
}

.card__title {
  margin: 0;
  font-size: 20px;
  color: #333;
  font-weight: 700;
}


.card__description {
  margin: 10px 0 10px;
  font-size: 12px;
  color: #777;
  line-height: 1.4;
}

.card__button {
  padding: 15px;
  border-radius: 8px;
  background: #777;
  border: none;
  color: white;
}

.secondary {
  background: transparent;
  color: #777;
  border: 1px solid #777;
}
</style>
