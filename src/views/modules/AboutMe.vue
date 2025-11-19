<template>
  <section id="about-me"
    class="flex flex-col md:flex-row gap-8 justify-center items-center lg:w-[740px] mx-auto py-36 text-center text-black/80 dark:text-white/80 ">
    <div
      class="[&>p]:mb-4 [&>p>span]:text-blue-600  [&>p>strong]:font-semibold text-pretty order-2 md:order-1 md:text-left ">
      <h2
        class="text-xl sm:text-2xl md:text-4xl font-semibold mb-6 flex items-center text-center text-black/80 dark:text-white/80 px-4 md:px-0 transition hover:scale-110 flex-col sm:flex-row">
        <profile-check class="size-16 mb-2 sm:mr-2" />
        <span>Sobre Mi</span>
      </h2>
      <p>

        Me llamo Sebastián Tovar Chávez, soy estudiante de ingeniería en sistemas apasionado por la programación, desde
        los
        19 años cuando comencé mis estudios universitarios <span class="font-bold"> empece el el mundo de la
          programación gracias a mi
          formación técnico en sistemas durante la etapa de colegio</span>.
      </p>
      <p>
        Me caracterizo por estar en constante aprendizaje y mantener el hábito de ser autodidacta.
        <span class="font-bold">
          Algunos de mis éxitos incluyen colaborar en el desarrollo de la página web de COOTRANSHUILA LTDA y
          participación
          en el backend como
          desarrollador web.</span> Esta experiencia fue un gran avance me enseño sobre trabajo en equipo y
        progresodel dia a dia en el ámbito del desarrollo web.
      </p>

      <p>
        Mi objetivo es seguir aprendiendo,<span class="font-bold"> enfrentar nuevos desafíos y nunca rendirme, <em
            class="italic">incluso
            ante los obstáculos más difíciles.</em>Estoy comprometido con mi crecimiento</span> profesional y emocionado
        por las oportunidades que el mundo del desarrollo tiene para ofrecer.
      </p>
    </div>

    <img src="/img/sebas.jpg" class="rounded-full size-64 order-1 md:order-2  mx-auto md:mx-0" />

  </section>
</template>

<script>
import profileCheckVue from '@/components/icons/profileCheck.vue'
export default {
  components: { profileCheckVue }

}
</script>

<style></style>
