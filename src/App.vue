<template>
  <NavBar />
  <HeadPage />
  <ExperiencePage />
  <SkillsPage />
  <ProjectsPage />
  <EducationPage />
  <ContactPage />
</template>

<script>
import NavBar from "@/components/NavBar.vue";
import HeadPage from "@/components/HeadPage.vue";
import ExperiencePage from "@/components/ExperiencePage.vue";
import SkillsPage from "@/components/SkillsPage.vue";
import ProjectsPage from "@/components/ProjectsPage.vue";
import EducationPage from "@/components/EducationPage.vue";
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
