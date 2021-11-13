<template>
  <div class="wrap">
    <div class="head">
      <h1>Skills</h1>
      <div class="skills">
        <div class="skill">
          <h2>Programming Languages</h2>
          <div class="level">
            <h3>HTML/CSS</h3>
            <div class="progress">
              <div class="bar">
                <p class="value" style="width: 200px"></p>
              </div>
              <span>100%</span>
            </div>
          </div>
          <div class="level">
            <h3>JAVASCRIPT</h3>
            <div class="progress">
              <div class="bar">
                <p class="value" style="width: 200px"></p>
              </div>
              <span>100%</span>
            </div>
          </div>
          <div class="level">
            <h3>PYTHON</h3>
            <div class="progress">
              <div class="bar">
                <p class="value" style="width: 180px"></p>
              </div>
              <span>90%</span>
            </div>
          </div>
          <div class="level">
            <h3>C/C++</h3>
            <div class="progress">
              <div class="bar">
                <p class="value" style="width: 160px"></p>
              </div>
              <span>80%</span>
            </div>
          </div>
        </div>
        <div class="skill">
          <h2>Frameworks/Libraries</h2>
          <div class="level">
            <h3>VUE.JS</h3>
            <div class="progress">
              <div class="bar">
                <p class="value" style="width: 200px"></p>
              </div>
              <span>100%</span>
            </div>
          </div>
          <div class="level">
            <h3>REACT JS</h3>
            <div class="progress">
              <div class="bar">
                <p class="value" style="width: 200px"></p>
              </div>
              <span>100%</span>
            </div>
          </div>
          <div class="level">
            <h3>NODE.JS/EXPRESS.JS/SOCKET.IO</h3>
            <div class="progress">
              <div class="bar">
                <p class="value" style="width: 200px"></p>
              </div>
              <span>100%</span>
            </div>
          </div>
          <div class="level">
            <h3>ELECTRON.JS</h3>
            <div class="progress">
              <div class="bar">
                <p class="value" style="width: 160px"></p>
              </div>
              <span>80%</span>
            </div>
          </div>
          <div class="level">
            <h3>TENSORFLOW</h3>
            <div class="progress">
              <div class="bar">
                <p class="value" style="width: 120px"></p>
              </div>
              <span>60%</span>
            </div>
          </div>
        </div>
        <div class="skill">
          <h2>Softwares</h2>
          <div class="level">
            <h3>LINUX</h3>
            <div class="progress">
              <div class="bar">
                <p class="value" style="width: 180px"></p>
              </div>
              <span>90%</span>
            </div>
          </div>
          <div class="level">
            <h3>WINDOWS</h3>
            <div class="progress">
              <div class="bar">
                <p class="value" style="width: 180px"></p>
              </div>
              <span>90%</span>
            </div>
          </div>
          <div class="level">
            <h3>FIGMA</h3>
            <div class="progress">
              <div class="bar">
                <p class="value" style="width: 180px"></p>
              </div>
              <span>90%</span>
            </div>
          </div>
          <div class="level">
            <h3>GIT/GITHUB</h3>
            <div class="progress">
              <div class="bar">
                <p class="value" style="width: 180px"></p>
              </div>
              <span>90%</span>
            </div>
          </div>
          <div class="level">
            <h3>MICROSOFT OFFICE</h3>
            <div class="progress">
              <div class="bar">
                <p class="value" style="width: 140px"></p>
              </div>
              <span>70%</span>
            </div>
          </div>
        </div>
        <div class="skill">
          <h2>Languages</h2>
          <div class="level">
            <h3>MALAYALAM</h3>
            <div class="progress">
              <div class="bar">
                <p class="value" style="width: 200px"></p>
              </div>
              <span>100%</span>
            </div>
          </div>
          <div class="level">
            <h3>KONKINI</h3>
            <div class="progress">
              <div class="bar">
                <p class="value" style="width: 180px"></p>
              </div>
              <span>90%</span>
            </div>
          </div>
          <div class="level">
            <h3>ENGLISH</h3>
            <div class="progress">
              <div class="bar">
                <p class="value" style="width: 160px"></p>
              </div>
              <span>80%</span>
            </div>
          </div>
          <div class="level">
            <h3>HINDI</h3>
            <div class="progress">
              <div class="bar">
                <p class="value" style="width: 160px"></p>
              </div>
              <span>80%</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SkillsPage",
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
  padding: 100px 0;
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
  margin-bottom: 50px;
  text-shadow: 0 0 15px #d4d3b8;
}

h2 {
  margin-bottom: 20px;
  color: #fbae3c;
}

.skills {
  text-align: left;
  margin: 50px;
  background: rgba(0, 0, 0, 0.6);
  -webkit-backdrop-filter: blur(10px);
  backdrop-filter: blur(10px);
  border-radius: 20px;
  padding: 50px;
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
}

.level {
  margin: 20px;
}

.progress {
  display: grid;
  grid-template-columns: auto auto;
  width: fit-content;
}

.bar {
  width: 200px;
  height: 5px;
  border-radius: 10px;
  background: #333333;
  display: inline-block;
  margin: 10px;
}

.value {
  height: 5px;
  background: #9900ff;
  border-radius: 10px;
}

@media only screen and (max-width: 768px) {
  .wrap {
    padding: 50px 0;
  }

  h1 {
    font-size: 1.8em;
    margin-bottom: 10px;
  }

  h2 {
    font-size: 1.2em;
  }

  h3 {
    font-size: 1em;
  }

  .skills {
    padding: 0;
    background: transparent;
  }

  .skill {
    margin: 0 auto;
  }

  .level {
    margin: 20px 0;
  }
}

@media only screen and (max-width: 400px) {
  .skill {
    margin: 0 20px;
  }
}
</style>
