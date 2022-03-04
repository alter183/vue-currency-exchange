<script lang="ts">
  import SkillBlock from "./FooterSkils.vue";
  import SignatureBlock from "./FooterSignature.vue";

  export default {
    components: {
      SkillBlock,
      SignatureBlock,
    },
  }
</script>

<template>
  <footer class="py-4 text-center">
      <div class="container px-4 mx-auto">
        <SkillBlock />
        <SignatureBlock />
      </div>
    </footer>
</template>
