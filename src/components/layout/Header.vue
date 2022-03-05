<script lang="ts">
  import Logo from "./HeaderLogo.vue"
  import GithubButton from "./HeaderGithubButton.vue"

  export default {
    components: {
      Logo,
      GithubButton
    }
  }
</script>

<template>
  <header class="py-2 md:py-4 bg-slate-200">
      <div class="container px-4 mx-auto flex justify-center md:justify-between items-center">
        <Logo />
        <GithubButton link="https://github.com/alter183/vue-currency-exchange" />
      </div>
    </header>
</template>