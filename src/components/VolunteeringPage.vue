<template>
  <div class="wrap">
    <div class="head">
      <div>
        <h1>Volunteering</h1>
        <div class="card">
          <ul>
            <li>SCOUT AND GUIDES (2018 - 2020)</li>
            <li>IEEE (2020 - NOW)</li>
            <li>ISTE (2021 - NOW)</li>
            <li>ROBOCEK GCE (2021 - NOW)</li>
            <li>IEEE WIE GCEK Event Organizing Team Member (2021)</li>
            <li>IEEE GCEK DEVCOM Web Development Mentor (2021)</li>
            <li>IEEE GCEK Web Development Team Member (2021)</li>
            <li>ROBOCEK GCEK Web Development Team Member (2021)</li>
          </ul>
        </div>
      </div>
      <div>
        <h1>Soft Skills</h1>
        <div class="card">
          <ul>
            <li>Good Communication And Teamwork Skill</li>
            <li>Good At Problem Solving</li>
            <li>Good At Managing Time And Tasks</li>
            <li>Dedicated To Task Till Task Ends</li>
            <li>Positive Mindset</li>
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
  padding: 100px 0;
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
  margin-bottom: 50px;
  text-shadow: 0 0 15px #d4d3b8;
}

h2 {
  margin-bottom: 20px;
  color: #fbae3c;
}

.card {
  text-align: center;
  margin: 50px;
}

ul {
  list-style-type: none;
}

li {
  height: auto;
  background: rgba(0, 0, 0, 0.6);
  -webkit-backdrop-filter: blur(10px);
  backdrop-filter: blur(10px);
  padding: 10px;
  border-radius: 30px;
  margin: 10px;
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
    padding: 50px 0;
  }

  .head {
    display: block;
  }

  h1 {
    font-size: 1.8em;
    margin-bottom: 10px;
  }
}
</style>
