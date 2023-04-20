<script setup lang="ts">
import Envelope from "~/components/svgs/Envelope.vue";
import Github from "~/components/svgs/Github.vue";
import Twitter from "~/components/svgs/Twitter.vue";
import LinkedIn from "~/components/svgs/LinkedIn.vue";

const year:Number = new Date().getFullYear();

</script>

<template>
  <footer id="contact">
    <span class="logo">
      <NuxtLink to="/">
        &lt;/emmo&gt;
      </NuxtLink>
    </span>
    <div class="socials">
      <a href="mailto:emmanolubiyi@gmail.com">
        <Envelope class="socialIcon" />
      </a>
      <a href="https://github.com/coded1guy"><Github class="socialIcon" /></a>
      <a href="https://twitter.com/lord_emmo" ><Twitter class="socialIcon" /></a>
      <a href="https://www.linkedin.com/in/emmanuel-olubiyi-2720a11b4/" target="_blank">
        <LinkedIn class="socialIcon" />
      </a>
    </div>
    <span>&copy; Emmanuel Olubiyi {{ year }}</span>
  </footer>
</template>

<style scoped>
@import url("assets/css/footer.css");
</style>