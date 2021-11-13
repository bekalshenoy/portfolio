<template>
  <NavBar />
  <HeadPage id="about" />
  <ExperiencePage id="experience" />
  <SkillsPage id="skills" />
  <ProjectsPage id="projects" />
  <EducationPage id="education" />
  <VolunteeringPage id="volunteering" />
  <ContactPage id="contact" />
</template>

<script>
import NavBar from "@/components/NavBar.vue";
import HeadPage from "@/components/HeadPage.vue";
import ExperiencePage from "@/components/ExperiencePage.vue";
import SkillsPage from "@/components/SkillsPage.vue";
import ProjectsPage from "@/components/ProjectsPage.vue";
import EducationPage from "@/components/EducationPage.vue";
import VolunteeringPage from "@/components/VolunteeringPage.vue";
import ContactPage from "@/components/ContactPage.vue";

export default {
  name: "App",

  components: {
    NavBar,
    HeadPage,
    ExperiencePage,
    SkillsPage,
    ProjectsPage,
    EducationPage,
    VolunteeringPage,
    ContactPage,
  },
};
</script>

<style>
* {
  font-family: Poppins, Helvetica, Arial, sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background: #ffffff;
  color: #333333;
}

h1,
h2,
h3 {
  font-family: Montserrat, Helvetica, Arial, sans-serif;
}
</style>
