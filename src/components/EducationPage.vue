<template>
  <div class="wrap">
    <div class="head">
      <h1>Education</h1>
      <div class="cards">
        <div class="card">
          <h2>B.Tech Computer Science And Engineering</h2>
          <h3>
            Government College Of Engineering Kannur (APJ Abdul Kalam
            Techno-logical University)
          </h3>
          <span>2020 - NOW</span>
        </div>
        <div class="card">
          <h2>PLUS TWO Biology Science</h2>
          <h3>S.N Trust’s H.S.S Thottada, Kannur (Kerala Board)</h3>
          <span>2020</span>
        </div>
        <div class="card">
          <h2>SSLC</h2>
          <h3>S.N Trust’s H.S.S Thottada, Kannur (Kerala Board)</h3>
          <span>2018</span>
        </div>
      </div>
      <h1>Courses Completed</h1>
      <div class="cards">
        <div class="card">
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
  color: #333333;
}

.card {
  width: 500px;
  min-height: 200px;
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
