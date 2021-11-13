<template>
  <div class="wrap">
    <div class="head">
      <div class="photo">
        <img
          src="../assets/me.webp"
          alt="my photo"
          @error="
            (e) => {
              e.onerror = null;
              e.src = '../assets/me.png';
            }
          "
        />
      </div>
      <div class="details">
        <div class="card">
          <h1>Ramnath Shenoy B</h1>
          <h3>Full Stack Web Developer / Data Science Enthusiast</h3>
          <p>
            Full Stack Web Developer with 4+ years of experience. Experienced in
            MEVN and MERN stack. Data Science and Machine Learning enthusiast
            with some experience in TENSORFLOW.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeadPage",
};
</script>

<style scoped>
.wrap {
  background: url("../assets/head-page.svg");
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  height: 100vh;
}

.head {
  width: 100%;
  max-width: 1920px;
  height: 100vh;
  margin: 0 auto;
  display: grid;
  grid-template-columns: 50% 50%;
  place-items: center;
  color: #ffffff;
  text-align: center;
}

img {
  border-radius: 50%;
  border: 1px solid #fbae3c;
  width: 75%;
  height: auto;
  margin: 0 auto;
}

.details {
  margin: 20px;
}

.card {
  background: rgba(0, 0, 0, 0.6);
  -webkit-backdrop-filter: blur(10px);
  backdrop-filter: blur(10px);
  border-radius: 20px;
  padding: 50px;
}

h1 {
  font-size: 3.2em;
  margin-bottom: 10px;
  color: #fbae3c;
}

h3 {
  margin-bottom: 20px;
  text-shadow: 0 0 15px #d4d3b8;
}

p {
  text-align: left;
}

@media only screen and (max-width: 1080px) {
  img {
    width: 80%;
    height: auto;
  }

  .card {
    padding: 20px;
  }
}

@media only screen and (max-width: 768px) {
  img {
    width: 50%;
    height: auto;
  }

  .wrap {
    padding: 100px 0 50px 0;
    height: auto;
  }

  .head {
    display: block;
    height: auto;
  }

  h1 {
    font-size: 1.8em;
  }

  p {
    text-align: center;
  }
}
</style>
