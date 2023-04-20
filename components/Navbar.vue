<script setup lang="ts">
import MobileNavIcon from "~/components/svgs/MobileNavIcon.vue";

const showDropDown = ref(false);

const toggleDropDown = () => {
  showDropDown.value = !showDropDown.value;
}
</script>

<template>
  <nav>
      <span class="logo">
        <NuxtLink to="/">
          &lt;emmo&gt;
        </NuxtLink>
      </span>
    <div class="nav-cnt">
      <button id="menu" @click="toggleDropDown">
        <MobileNavIcon :is-open=showDropDown />
      </button>
      <ul class="nav-links" :class="[showDropDown ? 'show-links' : '' ]">
        <li>
          <NuxtLink to="#about" class="active">About</NuxtLink>
        </li>
        <li>
          <NuxtLink to="#experience">Experience</NuxtLink>
        </li>
        <li>
          <NuxtLink to="#projects">Projects</NuxtLink>
        </li>
        <li>
          <NuxtLink to="#contact">Contact</NuxtLink>
        </li>
      </ul>
    </div>
  </nav>
</template>

<style scoped>
@import "assets/css/navbar.css";
</style>