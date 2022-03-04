<script lang="ts">
  import Header from "./Header.vue";
  import Footer from "./Footer.vue";

  export default {
    components: {
      Header,
      Footer,
    },
  }
</script>

<template>
    <Header />
    <main class="grow flex">
      <div class="container px-4 py-8 mx-auto self-center">
        <slot></slot>
      </div>
    </main>
    <Footer />
</template>