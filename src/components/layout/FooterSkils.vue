<script lang="ts">
  import { defineComponent } from 'vue';

  declare interface Skills {
    title: string,
    link: string,
    description: string
  }

  export default defineComponent({
    data(){
      return {
        skills: [
          {
            title: "Vue",
            link: "https://vuejs.org/",
            description: "Прогрессивный JavaScript фреймворк для создания пользовательских интерфейсов."
          },
          {
            title: "TailwindCSS",
            link: "https://tailwindcss.com/",
            description: "CSS-фреймворк, предлагающий обширный каталог классов и инструментов для облегчения стилизации сайта или приложения."
          }, 
          {
            title: "Git",
            link: "https://git-scm.com/",
            description: "Распределённая система управления версиями."
          },
          {
            title: "TypeScript",
            link: "https://www.typescriptlang.org/",
            description: "Язык программирования, позиционируемый как средство разработки веб-приложений, расширяющее возможности JavaScript."
          }, 
          {
            title: "SASS",
            link: "https://sass-lang.com/",
            description: "Метаязык на основе CSS, предназначенный для увеличения уровня абстракции CSS кода и упрощения файлов каскадных таблиц стилей."
          },
        ] as Skills[],
      }
    }
  });

</script>

<template>
  <p class="mb-4">
    Проект сделан для демонстрации навыков:
    <ul class="list-none">
      <li v-for="skill in skills" :key="skill.title"
          class="inline tehnology-list">
        <a v-bind:href="skill.link" v-bind:title="skill.description" target="_blank" rel="nofollow"
            class="underline decoration-pink-500 hover:text-pink-500 active:text-pink-700 transition-colors">
            {{ skill.title }}
        </a>
      </li>
    </ul>
  </p>
</template>

<style lang="sass">
  .tehnology-list 
    &::after
      content: ", "
    &:last-child::after
      content: none
</style>