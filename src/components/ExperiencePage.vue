<template>
  <div class="wrap">
    <div class="head">
      <h1>Experience</h1>
      <div class="cards">
        <div class="card">
          <h2>Front-End Developer Intern</h2>
          <h3>ATG (Across the Globe)</h3>
          <span>9/2021 - NOW</span>
          <br /><br />
          <p>Creating and managing websites</p>
        </div>
        <div class="card">
          <h2>Full-Stack Developer</h2>
          <h3>CESSE, Government College Of Engineering Kannur</h3>
          <span>5/2021 - NOW</span>
          <br /><br />
          <p>
            Helping in carbon neutral project of CESSE (Centre of Excellence in
            SYSTEMS, ENERGY & ENVIRONMENT), Government College of Engineering
            Kannur
          </p>
        </div>
        <div class="card">
          <h2>Web Developement Team Member</h2>
          <h3>IEEE WIE Kerala</h3>
          <span>3/2021 - NOW</span>
          <br /><br />
          <p>Helping in maintenance of WIE Kerala website</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ExperiencePage",
};
</script>

<style scoped>
.wrap {
  background: url("../assets/experience-page.svg");
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
  color: #333333;
}

.card {
  width: 500px;
  min-height: 300px;
  display: inline-block;
  overflow: hidden;
  margin: 20px;
  padding: 20px;
  border-radius: 20px;
  background: rgba(255, 255, 255, 0.8);
  -webkit-backdrop-filter: blur(10px);
  backdrop-filter: blur(10px);
  box-shadow: 0 0 0.5em 0.0625em rgba(0, 0, 0, 0.1);
  transition: all 0.5s ease-out;
}

.card:hover {
  background: rgba(255, 255, 255, 0.9);
  transition: all 0.25s ease-out;
}

h1 {
  font-size: 3.2em;
  margin-bottom: 50px;
  text-shadow: 0 0 15px #d4d3b8;
  color: #ffffff;
}

h2 {
  margin-bottom: 10px;
  color: #560090;
}

h3 {
  margin-bottom: 20px;
  color: #9900ff;
}

span {
  background: #fbae3c;
  padding: 5px 10px;
  color: #ffffff;
  border-radius: 5px;
}

@media only screen and (max-width: 1080px) {
  .card {
    max-width: 300px;
    min-height: 400px;
    overflow: hidden;
  }
}

@media only screen and (max-width: 768px) {
  .wrap {
    padding: 50px 0;
  }

  .card {
    width: auto;
    overflow: hidden;
  }

  h1 {
    font-size: 1.8em;
    margin-bottom: 10px;
  }
}
</style>
