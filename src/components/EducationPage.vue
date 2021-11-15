<template>
  <div class="wrap">
    <div class="head">
      <h1>Education</h1>
      <div class="cards">
        <div
          class="card"
          data-aos="zoom-in-up"
          data-aos-duration="1000"
          data-aos-easing="ease-out"
        >
          <h2>B.Tech Computer Science And Engineering</h2>
          <h3>
            Government College Of Engineering Kannur (APJ Abdul Kalam
            Techno-logical University)
          </h3>
          <span>2020 - NOW</span>
        </div>
        <div
          class="card"
          data-aos="zoom-in-up"
          data-aos-duration="1000"
          data-aos-easing="ease-out"
        >
          <h2>PLUS TWO Biology Science</h2>
          <h3>S.N Trust’s H.S.S Thottada, Kannur (Kerala Board)</h3>
          <span>2020</span>
        </div>
        <div
          class="card"
          data-aos="zoom-in-up"
          data-aos-duration="1000"
          data-aos-easing="ease-out"
        >
          <h2>SSLC</h2>
          <h3>S.N Trust’s H.S.S Thottada, Kannur (Kerala Board)</h3>
          <span>2018</span>
        </div>
      </div>
      <h1>Courses Completed</h1>
      <div class="cards">
        <div
          class="card"
          data-aos="zoom-in-up"
          data-aos-duration="1000"
          data-aos-easing="ease-out"
        >
          <h2>Neural Networks and Deep Learning</h2>
          <h3>by DeepLearning.AI(Andrew Ng)</h3>
          <span>2021</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "EducationPage",
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
}

.card {
  width: 31rem;
  min-height: 12.5rem;
  display: inline-block;
  overflow: hidden;
  margin: 1.25rem;
  padding: 1.25rem;
  border-radius: 1rem;
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
  padding: 0.25px 0.5rem;
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
  }

  .card {
    width: auto;
    overflow: hidden;
    min-height: 12.5rem;
  }

  h1 {
    font-size: 1.8em;
    margin-bottom: 0.5rem;
  }

  h2 {
    font-size: 1.2em;
  }

  h3 {
    font-size: 0.8em;
  }
}
</style>
