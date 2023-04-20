<template>
  <section id="projects">
    <h2>My Projects</h2>
    <div class="project-content">
      <ProjectCard
          project-title="RadioAdSpread"
          project-link="https://radioadspread.com/"
          project-github=""
          project-desc="I contributed to the development of the frontend implementation of the RadioAdspread web-app."
          project-lang="React, Next, JS"
      />
      <ProjectCard
          project-title="NewFrontiers"
          project-link="https://www.newfrontierslearning.com/"
          project-github=""
          project-desc="I worked with a team-mate at Dumela Corp to build this website for our client, NewFrontiers."
          project-lang="Wix website builder"
      />
      <ProjectCard
          project-title="NewFrontiers LMS"
          project-link="https://lms.newfrontierslearning.com/"
          project-github=""
          project-desc="I maintain and serve as a technical support engineer for this LMS. The LMS was developed by Dumela Corp for one of their client, NewFrontiers."
          project-lang="moodle, BigBlueButton, PHP"
      />
      <ProjectCard
          project-title="Niphi Global"
          project-link="https://niphiglobal.com/"
          project-github=""
          project-desc="I worked with a product designer, to develop this website for a client. This was a freelance work."
          project-lang="HTML, CSS, JS"
      />
      <ProjectCard
          project-title="Portfolio"
          project-link="https://emmanuel-olubiyi.vercel.app/"
          project-github=""
          project-desc="I designed and developed this portfolio website for myself."
          project-lang="Nuxt, CSS, TS"
      />
      <ProjectCard
          project-title="Wiki Search"
          project-link="https://wiki-search-app-delta.vercel.app/"
          project-github="https://github.com/coded1guy/Wiki-Search-App"
          project-desc="I designed and created this website during a coding challenge. It uses wiki's API to get results based on a user's search."
          project-lang="HTML, CSS, JS"
      />
    </div>
  </section>
</template>

<style>
.project-content {
  margin-top: 20px;
  display: flex;
  flex-flow: column nowrap;
  justify-content: center;
  gap: 30px;
  align-items: center;
}
@media screen and (min-width: 650px) {
  .project-content {
    display: flex;
    flex-flow: row wrap;
    justify-content: space-between;
    align-items: center;
  }
}
</style>
