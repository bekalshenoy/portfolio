<template>
  <div class="wrap">
    <div class="head">
      <div class="photo">
        <img
          src="../assets/me.webp"
          alt="my photo"
          data-aos="fade"
          data-aos-duration="1500"
          @error="
            (e) => {
              e.onerror = null;
              e.src = '../assets/me.png';
            }
          "
        />
      </div>
      <div
        class="details"
        data-aos="fade"
        data-aos-duration="1000"
        data-aos-delay="600"
      >
        <div class="card">
          <h1
            data-aos="fade-up"
            data-aos-duration="1000"
            data-aos-easing="ease-out"
          >
            Ramnath Shenoy B
          </h1>
          <h3
            data-aos="fade-up"
            data-aos-duration="1000"
            data-aos-delay="200"
            data-aos-easing="ease-out"
          >
            Full Stack Web Developer / Data Science Enthusiast
          </h3>
          <p
            data-aos="fade-up"
            data-aos-duration="1000"
            data-aos-delay="400"
            data-aos-easing="ease-out"
          >
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
  margin: 1.25rem;
}

.card {
  background: rgba(0, 0, 0, 0.6);
  -webkit-backdrop-filter: blur(0.5rem);
  backdrop-filter: blur(0.5rem);
  border-radius: 1.25rem;
  padding: 3rem;
}

h1 {
  font-size: 3.2em;
  margin-bottom: 0.5rem;
  color: #fbae3c;
}

h3 {
  margin-bottom: 1.25rem;
  text-shadow: 0 0 1rem #d4d3b8;
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
    padding: 1.25rem;
  }
}

@media only screen and (max-width: 768px) {
  img {
    width: 50%;
    height: auto;
  }

  .wrap {
    padding: 6rem 0 3rem 0;
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
