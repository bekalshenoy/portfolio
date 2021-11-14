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
import AOS from "aos";
import "aos/dist/aos.css";
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

  mounted() {
    AOS.init();
  },
};
</script>

<style>
* {
  font-family: Poppins, Helvetica, Arial, sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  user-select: none;
}

::-webkit-scrollbar {
  width: 0.5rem;
  border-radius: 0.5rem;
}

::-webkit-scrollbar-track {
  background: #333333;
  border-radius: 0.5rem;
}

::-webkit-scrollbar-thumb {
  background: #fbae3c;
  background: linear-gradient(
    180deg,
    rgba(153, 0, 255, 1) 0%,
    rgba(86, 0, 144, 1) 35%,
    rgba(251, 174, 60, 1) 100%
  );
  border-radius: 0.5rem;
}

html {
  scroll-behavior: smooth;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  overflow-x: hidden;
}

body {
  background: #000000;
  color: #333333;
  overflow-x: hidden;
}

h1,
h2,
h3 {
  font-family: Montserrat, Helvetica, Arial, sans-serif;
}
</style>
