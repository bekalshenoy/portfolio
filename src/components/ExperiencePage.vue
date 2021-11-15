<template>
  <div class="wrap">
    <div class="head">
      <h1>Experience</h1>
      <div class="cards">
        <div
          class="card"
          data-aos="zoom-in-up"
          data-aos-duration="1000"
          data-aos-easing="ease-out"
        >
          <h2>Front-End Developer Intern</h2>
          <h3>ATG (Across the Globe)</h3>
          <span>9/2021 - NOW</span>
          <br /><br />
          <p>Creating and managing websites</p>
        </div>
        <div
          class="card"
          data-aos="zoom-in-up"
          data-aos-duration="1000"
          data-aos-easing="ease-out"
        >
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
        <div
          class="card"
          data-aos="zoom-in-up"
          data-aos-duration="1000"
          data-aos-easing="ease-out"
        >
          <h2>Web Development Team Member</h2>
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

.card {
  width: 31rem;
  min-height: 18.75rem;
  display: inline-block;
  overflow: hidden;
  margin: 1.25rem;
  padding: 1.25rem;
  border-radius: 1.25rem;
  background: rgba(0, 0, 0, 0.6);
  border: 1px solid #fbae3c;
  -webkit-backdrop-filter: blur(0.5rem);
  backdrop-filter: blur(0.5rem);
  box-shadow: 0 0 0.5em 0.0625rem rgba(0, 0, 0, 0.1);
  transition: all 0.5s ease-out;
}

.card:hover {
  border: 1px solid #9900ff;
  transition: all 0.5s ease-out;
}

h1 {
  font-size: 3.2em;
  margin-bottom: 3rem;
  text-shadow: 0 0 1rem #d4d3b8;
  color: #ffffff;
}

h2 {
  margin-bottom: 0.5rem;
  color: #fbae3c;
}

h3 {
  margin-bottom: 1.25rem;
  color: #ffffff;
}

span {
  background: #fbae3c;
  background: linear-gradient(
    90deg,
    rgba(153, 0, 255, 1) 0%,
    rgba(86, 0, 144, 1) 35%,
    rgba(251, 174, 60, 1) 100%
  );
  padding: 0.25rem 0.5rem;
  color: #ffffff;
  border-radius: 0.25rem;
}

@media only screen and (max-width: 1080px) {
  .card {
    max-width: 18.75rem;
    min-height: 25rem;
    overflow: hidden;
  }
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

  .card {
    width: auto;
    overflow: hidden;
  }

  h1 {
    font-size: 1.8em;
    margin-bottom: 0.5rem;
  }
}
</style>
