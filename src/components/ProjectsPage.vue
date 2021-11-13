<template>
  <div class="wrap">
    <div class="head">
      <h1>Projects</h1>
      <div class="cards">
        <div class="card">
          <h2>Carbon Neutral Project</h2>
          <span>2021 - NOW</span>
          <br /><br />
          <p>
            A Project Started To Make Colleges Under APJ Abdul Kalam
            Technological University Carbon Neutral Using Machine Learning And
            AI
          </p>
        </div>
        <div class="card">
          <h2>Event Management Website</h2>
          <span>2021</span>
          <br /><br />
          <p>
            Created a Event Management Website For 'Build From Zero' Event
            Organized By TinkerHub GCEK
          </p>
          <button>
            <a href="https://bit.ly/3zWkFKq" target="_blank">View Source</a>
          </button>
        </div>
        <div class="card">
          <h2>Class Forum</h2>
          <span>2021</span>
          <br /><br />
          <p>
            Created A Class Forum For Government College Of Engineering Kannur
            CSE 2020 Batch.
          </p>
          <button>
            <a href="https://bit.ly/3ux5PrX" target="_blank">View Source</a>
          </button>
        </div>
        <div class="card">
          <h2>Sticky Notes</h2>
          <span>2017 - 2020</span>
          <br /><br />
          <p>
            Created A Sticky Notes Application For Linux. Went Up To 10000 Daily
            User
          </p>
          <button>
            <a href="https://bit.ly/3xW1UHd" target="_blank">View Source</a>
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
  background: url("../assets/head-page.svg");
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
  margin-bottom: 15px;
  color: #560090;
}

span {
  background: #fbae3c;
  padding: 5px 10px;
  color: #ffffff;
  border-radius: 5px;
}

button {
  width: 150px;
  border-radius: 10px;
  padding: 10px;
  margin: 20px;
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
  background: rgba(255, 255, 255, 0.6);
  -webkit-backdrop-filter: blur(10px);
  backdrop-filter: blur(10px);
  border: 1px solid #fbae3c;
  transition: all 0.5s ease-out;
}

button:hover a {
  color: #333333;
  transition: all 0.5s ease-out;
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
    width: 100%;
    width: auto;
    overflow: hidden;
  }

  h1 {
    font-size: 1.8em;
    margin-bottom: 10px;
  }
}
</style>
