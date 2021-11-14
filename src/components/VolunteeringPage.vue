<template>
  <div class="wrap">
    <div class="head">
      <div>
        <h1>Volunteering</h1>
        <div class="card">
          <ul>
            <li
              data-aos="fade-up"
              data-aos-duration="1000"
              data-aos-easing="ease-out"
            >
              SCOUT AND GUIDES (2018 - 2020)
            </li>
            <li
              data-aos="fade-up"
              data-aos-duration="1000"
              data-aos-easing="ease-out"
              data-aos-delay="50"
            >
              IEEE (2020 - NOW)
            </li>
            <li
              data-aos="fade-up"
              data-aos-duration="1000"
              data-aos-easing="ease-out"
              data-aos-delay="100"
            >
              ISTE (2021 - NOW)
            </li>
            <li
              data-aos="fade-up"
              data-aos-duration="1000"
              data-aos-easing="ease-out"
              data-aos-delay="150"
            >
              ROBOCEK GCE (2021 - NOW)
            </li>
            <li
              data-aos="fade-up"
              data-aos-duration="1000"
              data-aos-easing="ease-out"
              data-aos-delay="200"
            >
              IEEE WIE GCEK Event Organizing Team Member (2021)
            </li>
            <li
              data-aos="fade-up"
              data-aos-duration="1000"
              data-aos-easing="ease-out"
              data-aos-delay="250"
            >
              IEEE GCEK DEVCOM Web Development Mentor (2021)
            </li>
            <li
              data-aos="fade-up"
              data-aos-duration="1000"
              data-aos-easing="ease-out"
              data-aos-delay="300"
            >
              IEEE GCEK Web Development Team Member (2021)
            </li>
            <li
              data-aos="fade-up"
              data-aos-duration="1000"
              data-aos-easing="ease-out"
              data-aos-delay="350"
            >
              ROBOCEK GCEK Web Development Team Member (2021)
            </li>
          </ul>
        </div>
      </div>
      <div>
        <h1>Soft Skills</h1>
        <div class="card">
          <ul>
            <li
              data-aos="fade-up"
              data-aos-duration="1000"
              data-aos-easing="ease-out"
            >
              Good Communication And Teamwork Skill
            </li>
            <li
              data-aos="fade-up"
              data-aos-duration="1000"
              data-aos-easing="ease-out"
              data-aos-delay="50"
            >
              Good At Problem Solving
            </li>
            <li
              data-aos="fade-up"
              data-aos-duration="1000"
              data-aos-easing="ease-out"
              data-aos-delay="100"
            >
              Good At Managing Time And Tasks
            </li>
            <li
              data-aos="fade-up"
              data-aos-duration="1000"
              data-aos-easing="ease-out"
              data-aos-delay="150"
            >
              Dedicated To Task Till Task Ends
            </li>
            <li
              data-aos="fade-up"
              data-aos-duration="1000"
              data-aos-easing="ease-out"
              data-aos-delay="200"
            >
              Positive Mindset
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "VolunteeringPage",
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
  padding: 6rem 0;
}

.head {
  width: 100%;
  max-width: 1920px;
  margin: 0 auto;
  text-align: center;
  color: #ffffff;
  display: grid;
  grid-template-columns: 50% 50%;
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

.card {
  text-align: center;
  margin: 3rem;
}

ul {
  list-style-type: none;
}

li {
  height: auto;
  background: rgba(0, 0, 0, 0.6);
  -webkit-backdrop-filter: blur(0.5rem);
  backdrop-filter: blur(0.5rem);
  padding: 0.5rem;
  border-radius: 2rem;
  margin: 0.5rem;
  border: 1px solid #fbae3c;
  transition: all 0.5s ease-out;
}

li:hover {
  border: 1px solid #9900ff;
  transition: all 0.5s ease-out;
}

@media only screen and (max-width: 1080px) {
  li {
    font-size: 0.8em;
  }
}

@media only screen and (max-width: 768px) {
  .wrap {
    padding: 3rem 0;
  }

  .head {
    display: block;
  }

  h1 {
    font-size: 1.8em;
    margin-bottom: 0.5rem;
  }
}
</style>
