<template>
  <div class="wrap">
    <div class="head">
      <h1>Skills</h1>
      <div class="skills">
        <div class="skill">
          <h2>Programming Languages</h2>
          <div class="level">
            <h3>HTML/CSS</h3>
            <ProgressBar value="100" />
          </div>
          <div class="level">
            <h3>JAVASCRIPT</h3>
            <ProgressBar value="100" />
          </div>
          <div class="level">
            <h3>PYTHON</h3>
            <ProgressBar value="90" />
          </div>
          <div class="level">
            <h3>C/C++</h3>
            <ProgressBar value="80" />
          </div>
        </div>
        <div class="skill">
          <h2>Frameworks/Libraries</h2>
          <div class="level">
            <h3>VUE.JS</h3>
            <ProgressBar value="100" />
          </div>
          <div class="level">
            <h3>REACT JS</h3>
            <ProgressBar value="100" />
          </div>
          <div class="level">
            <h3>NODE.JS/EXPRESS.JS/SOCKET.IO</h3>
            <ProgressBar value="100" />
          </div>
          <div class="level">
            <h3>ELECTRON.JS</h3>
            <ProgressBar value="80" />
          </div>
          <div class="level">
            <h3>TENSORFLOW</h3>
            <ProgressBar value="60" />
          </div>
        </div>
        <div class="skill">
          <h2>Softwares</h2>
          <div class="level">
            <h3>LINUX</h3>
            <ProgressBar value="90" />
          </div>
          <div class="level">
            <h3>WINDOWS</h3>
            <ProgressBar value="90" />
          </div>
          <div class="level">
            <h3>FIGMA</h3>
            <ProgressBar value="90" />
          </div>
          <div class="level">
            <h3>GIT/GITHUB</h3>
            <ProgressBar value="90" />
          </div>
          <div class="level">
            <h3>MICROSOFT OFFICE</h3>
            <ProgressBar value="70" />
          </div>
        </div>
        <div class="skill">
          <h2>Languages</h2>
          <div class="level">
            <h3>MALAYALAM</h3>
            <ProgressBar value="100" />
          </div>
          <div class="level">
            <h3>KONKINI</h3>
            <ProgressBar value="90" />
          </div>
          <div class="level">
            <h3>ENGLISH</h3>
            <ProgressBar value="80" />
          </div>
          <div class="level">
            <h3>HINDI</h3>
            <ProgressBar value="80" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ProgressBar from "@/components/ProgressBar.vue";

export default {
  name: "SkillsPage",

  components: {
    ProgressBar,
  },
};
</script>

<style scoped>
.wrap {
  background: url("../assets/skills-page.svg");
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  height: auto;
  padding: 6rem 0;
}

.head {
  width: 100%;
  max-width: 1920px;
  margin: 0 auto;
  text-align: center;
  color: #ffffff;
}

h1 {
  font-size: 3.2em;
  margin-bottom: 3rem;
  text-shadow: 0 0 1rem #d4d3b8;
}

h2 {
  margin-bottom: 1.25rem;
  color: #fbae3c;
}

.skills {
  text-align: left;
  margin: 3rem;
  background: rgba(0, 0, 0, 0.6);
  border: 1px solid #fbae3c;
  -webkit-backdrop-filter: blur(0.5rem);
  backdrop-filter: blur(0.5rem);
  border-radius: 1rem;
  padding: 3rem;
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(22rem, 1fr));
}

.level {
  margin: 1.25rem;
}

@media only screen and (max-width: 768px) {
  .wrap {
    padding: 3rem 0;
    background: url("../assets/experience-page.svg");
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
  }

  h1 {
    font-size: 1.8em;
    margin-bottom: 0.5rem;
  }

  h2 {
    font-size: 1em;
  }

  h3 {
    font-size: 0.8em;
  }

  .skills {
    padding: 3rem 0;
    border: 1px solid #fbae3c;
  }

  .skill {
    margin: 0 auto;
  }

  .level {
    margin: 1.25rem 0;
  }
}

@media only screen and (max-width: 400px) {
  .skill {
    margin: 0 1.5rem;
  }
}
</style>
