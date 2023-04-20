<script setup lang="ts">
import GoToLink from "~/components/svgs/GoToLink.vue";
import Github from "~/components/svgs/Github.vue";

defineProps({
  projectTitle: String,
  projectLink: String,
  projectGithub: String,
  projectDesc: String,
  projectLang: String,
})
</script>

<template>
  <div class="project-card">
    <div class="project-heading">
      <h3>{{projectTitle}}</h3>
      <div>
        <a :href=projectGithub target="_blank" v-if=projectGithub title="go to github repo">
          <Github />
        </a>
        <a :href=projectLink target="_blank" title="go to live site">
          <GoToLink />
        </a>
      </div>
    </div>
    <p class="project-description">
      {{projectDesc}}
    </p>
    <ul class="skills">
      <li v-for="(lang, index) in projectLang.split(',')" :key="index" v-if=projectLang>
        {{lang}}
      </li>
    </ul>
  </div>
</template>

<style scoped>
.project-card {
  width: 100%;
  max-width: 360px;
  background: var(--heavy-blue);
  border-radius: 5px;
  padding: 20px;
  box-shadow: 4px 4px 1px rgba(242,174,48,.7);
  display: flex;
  flex-flow: column nowrap;
  gap: 18px;
}
.project-heading {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.project-heading h3 {

}
.project-heading > div {
  display: flex;
  gap: 10px;
}
.project-heading a {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 25px;
  height: 25px;
  cursor: pointer;
}
.project-heading a > svg {
  display: block;
  width: 80%;
  height: auto;
  fill: var(--dirty-white);
  transition: .2s ease;
}
.project-heading a > svg:hover {
  width: 100%;
  fill: var(--gold);
}
div.project-card p.project-description {
  font-size: 15px;
  color: var(--dirty-white);
}
.skills {
  display: flex;
  flex-flow: row wrap;
  gap: 7px;
}
.skills li {
  background: transparent;
  display: inline-block;
  color: var(--dirty-white);
  border: 1px solid var(--gold);
  border-radius: 5px;
  padding: 5px 10px;
  font-family: var(--logo-font);
  font-size: 13px;
  cursor: pointer;
  transition: .3s ease;
}
.skills li:hover {
  background: var(--gold);
  color: var(--dirty-white);
}

@media screen and (min-width: 650px) {
  .project-card {
    max-width: 280px;
  }
  @media screen and (min-width: 730px) {
    .project-card {
      max-width: 300px;
    }
    @media screen and (min-width: 830px) {
      .project-card {
        max-width: 350px;
      }
    }
  }
}
</style>
