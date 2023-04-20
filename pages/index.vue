<script setup lang="ts">
// import { gsap } from 'gsap'
// import { TextPlugin } from 'gsap/TextPlugin'
// import { ScrollTrigger } from 'gsap/ScrollTrigger'
//
// if (process.client) {
//   gsap.registerPlugin(TextPlugin, ScrollTrigger)
// }
import MyProjects from "~/components/MyProjects.vue";
</script>

<template>
  <main>
    <HomeIntro />
    <div class="main-contents">
      <AboutMe />
      <MyExperiences />
      <MyProjects />
    </div>
  </main>
</template>

<style>
  main {
    display: flex;
    flex-flow: column nowrap;
  }
  .main-contents {
    width: 100%;
    padding: 30px 0 0 0;
  }
  .main-contents > section {
    padding: 30px 30px;
  }
  .main-contents > section h2 {
    color: var(--dirty-white);
    text-shadow: 3px 3px 1px rgba(242,174,48,.4);
    font-size: 24px;
  }
  .main-contents > section p {
    color: var(--dirty-white);
  }
  .main-contents > section:nth-child(odd) {
    background: var(--dirty-white);
  }
  .main-contents > section:nth-child(odd) h2 {
    color: var(--heavy-blue);
  }
  .main-contents > section:nth-child(odd) p {
    color: var(--heavy-blue);
  }
  /* responsive design for bigger screens */
  @media screen and (min-width: 700px) {
    .main-contents > section {
      padding: 35px 50px;
    }
    .main-contents > section h2 {
      font-size: 30px;
    }
  }
</style>
