<template>
  <section id="experience">
    <h2>My Experience</h2>
    <ul class="experience-list">
      <li class="exp-desc">
        I was introduced to <strong>Frontend Web Development</strong> in 2016 by
        some alumni of my secondary school, I then went on to learn <strong>HTML</strong>,
        <strong>CSS</strong> and <strong>JS</strong> from
        <a href="www.codecademy.com" target="_blank">codecademy</a> and
        <a href="https://www.freecodecamp.org/learn" target="_blank">freecodecamp</a>.
      </li>
      <li class="exp-desc">
        Across late 2016 to 2017 I got into a “learning craze” where I started tutorials in
        languages like <strong>ruby</strong>, <strong> C#</strong>, <strong> C++</strong>,
        <strong> Python</strong> and <strong> GO</strong>.<br />
        I didn’t finish the tutorials as they got too complex for me to understand 😗.
      </li>
      <li class="exp-desc">
        I was introduced to <strong>SCRATCH</strong> programming in 2017 and I got interested
        in it, focused primarily  on it alongside <strong>HTML</strong>, <strong>CSS</strong> and
        <strong>JavaScript</strong> till I left secondary school in 2019.
      </li>
      <li class="exp-desc">
        Early 2020, I resumed my university education at the University of Lagos,
        where I got associated with groups like <strong>Google Developer Students Club (GDSC)</strong>
        and <strong>Engineering Career Expo (ECX)</strong> which helped me to
        advance and start a career in <strong>Frontend Development</strong>.
      </li>
      <li class="exp-desc">
        In 2020, during the <strong>COVID-19</strong> break, I participated in different
        <strong>Bootcamps</strong>, <strong>internships</strong> and <strong>coding sprint/challenge</strong>.
      </li>
      <li class="exp-desc">
        Later in 2020, I got involved in 2 internships, one was with a Nigeria-based company called
        <strong>Space Universe</strong>, the other was a contract internship with a company called
        <strong>Dumela Corp</strong>, which is based in Seattle, WA.
      </li>
      <li class="exp-desc">
        In <strong>Space Universe</strong>, I worked on optimising the <strong>frontend</strong> of the initial
        landing page of their child company, <strong>RadioAdSpread</strong>, while at <strong>Dumela Corp</strong>
        I worked on their client <strong>websites</strong> and <strong>web-apps</strong>.
      </li>
      <li class="exp-desc">
        In 2021, I transitioned to a <strong>Technical Support Engineer</strong> role at a child company of
        <strong>Space Universe</strong>, <strong>PopAdlink</strong>, where I managed their <strong>web-apps</strong>
        and worked on providing solutions to <strong>technical problems</strong> faced on the web-app by customers.
      </li>
      <li class="exp-desc">
        In 2021, I transitioned from being a <strong>Software Engineer Intern</strong> to being a
        <strong>Software Engineer</strong> at <strong>Dumela Corp</strong>.
      </li>
      <li class="exp-desc">
        In 2022, I worked as a <strong>frontend developer</strong> at <strong>Space Universe</strong>, where I
        developed <strong>websites</strong> and <strong>web-apps</strong> for some of their child
        companies (<strong>RadioAdspread</strong>, <strong>DevPartners</strong>).
      </li>
    </ul>
  </section>
</template>

<style scoped>
.experience-list {
  display: flex;
  flex-flow: column nowrap;
  justify-content: center;
  align-items: center;
  gap: 30px;
  margin-top: 20px;
}
.exp-desc {
  width: 100%;
  max-width: 360px;
  background: var(--dirty-white);
  padding: 20px;
  border-radius: 5px;
  color: var(--heavy-blue);
  transition: .5s ease;
  box-shadow: 4px 4px 1px rgba(242,174,48,.7);
}
.exp-desc a {
  text-decoration: underline;
}
@media screen and (min-width: 650px) {
  .experience-list {
    display: flex;
    flex-flow: row wrap;
    justify-content: space-between;
    align-items: center;
  }
  .exp-desc {
    max-width: 280px;
  }
  @media screen and (min-width: 730px) {
    .exp-desc {
      max-width: 300px;
    }
    @media screen and (min-width: 830px) {
      .exp-desc {
        max-width: 350px;
      }
    }
  }
}
</style>
