<template>
  <div class="wrap">
    <div class="head">
      <h1>Projects</h1>
      <div class="cards">
        <div
          class="card"
          data-aos="zoom-in-up"
          data-aos-duration="1000"
          data-aos-easing="ease-out"
        >
          <h2>Carbon Neutral Project</h2>
          <span>2021 - NOW</span>
          <br /><br />
          <p>
            A Project Started To Make Colleges Under APJ Abdul Kalam
            Technological University Carbon Neutral Using Machine Learning And
            AI
          </p>
        </div>
        <div
          class="card"
          data-aos="zoom-in-up"
          data-aos-duration="1000"
          data-aos-easing="ease-out"
        >
          <h2>Event Management Website</h2>
          <span>2021</span>
          <br /><br />
          <p>
            Created a Event Management Website For 'Build From Zero' Event
            Organized By TinkerHub GCEK
          </p>
          <button>
            <a href="https://bit.ly/3zWkFKq" target="_blank" rel="noopener"
              >View Source</a
            >
          </button>
        </div>
        <div
          class="card"
          data-aos="zoom-in-up"
          data-aos-duration="1000"
          data-aos-easing="ease-out"
        >
          <h2>Class Forum</h2>
          <span>2021</span>
          <br /><br />
          <p>
            Created A Class Forum For Government College Of Engineering Kannur
            CSE 2020 Batch.
          </p>
          <button>
            <a href="https://bit.ly/3ux5PrX" target="_blank" rel="noopener"
              >View Source</a
            >
          </button>
        </div>
        <div
          class="card"
          data-aos="zoom-in-up"
          data-aos-duration="1000"
          data-aos-easing="ease-out"
        >
          <h2>Sticky Notes</h2>
          <span>2017 - 2020</span>
          <br /><br />
          <p>
            Created A Sticky Notes Application For Linux. Went Up To 10000 Daily
            User
          </p>
          <button>
            <a href="https://bit.ly/3xW1UHd" target="_blank" rel="noopener"
              >View Source</a
            >
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProjectsPage",
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
  margin-bottom: 1rem;
  color: #fbae3c;
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

button {
  width: 9.25rem;
  border-radius: 0.5rem;
  padding: 0.5rem;
  margin: 1.25rem;
  outline: none;
  border: none;
  background: #ffffff;
  cursor: pointer;
  border: 1px solid transparent;
  transition: all 0.5s ease-out;
}

button a {
  color: #9900ff;
  text-decoration: none;
  transition: all 0.5s ease-out;
}

button:hover {
  background: rgba(0, 0, 0, 0.6);
  -webkit-backdrop-filter: blur(0.5rem);
  backdrop-filter: blur(0.5rem);
  border: 1px solid #fbae3c;

  transition: all 0.5s ease-out;
}

button:hover a {
  color: #ffffff;
  transition: all 0.5s ease-out;
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
