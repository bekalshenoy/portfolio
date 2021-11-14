<template>
  <div class="wrap">
    <div class="contact">
      <div class="head">
        <h1>Contact Me</h1>
        <div class="social">
          <a href="https://bit.ly/3xRYiGd" target="_blank" rel="noopener"
            ><img src="../assets/github.svg" alt="github"
          /></a>
          <a href="https://bit.ly/3txLPnx" target="_blank" rel="noopener"
            ><img src="../assets/linkedin.svg" alt="linkedin"
          /></a>
          <a
            href="https://twitter.com/bramnathshenoy"
            target="_blank"
            rel="noopener"
            ><img src="../assets/twitter.svg" alt="twitter"
          /></a>
        </div>
      </div>
      <div class="form">
        <input
          type="email"
          placeholder="Email"
          data-aos="fade-up"
          data-aos-duration="1000"
          data-aos-easing="ease-out"
        />
        <input
          type="text"
          placeholder="Subject"
          data-aos="fade-up"
          data-aos-duration="1000"
          data-aos-delay="100"
          data-aos-easing="ease-out"
        />
        <textarea
          placeholder="Description"
          data-aos="fade-up"
          data-aos-duration="1000"
          data-aos-delay="200"
          data-aos-easing="ease-out"
        ></textarea>
        <input
          type="button"
          value="Send"
          data-aos="fade-up"
          data-aos-duration="1000"
          data-aos-delay="300"
          data-aos-easing="ease-out"
        />
      </div>
      <span>&copy;Copyright Ramnath Shenoy B 2021</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "ContactPage",
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
  padding: 6rem 0;
}

.contact {
  width: 100%;
  max-width: 1920px;
  margin: 0 auto;
  display: grid;
  grid-template-columns: 50% 50%;
  place-items: center;
  color: #ffffff;
  text-align: center;
}

a {
  text-decoration: none;
  color: #ffffff;
  display: inline-block;
  cursor: pointer;
  padding: 0.5rem;
  transition: all 0.5s ease-out;
}

a:hover {
  opacity: 0.8;
  transition: all 0.5s ease-out;
}

h1 {
  font-size: 3.2em;
  margin-bottom: 0.5rem;
  text-shadow: 0 0 1rem #d4d3b8;
}

input,
textarea {
  display: block;
  margin: 1.25rem;
}

input[type="text"],
input[type="email"],
textarea {
  width: 30vw;
  height: 3rem;
  border-radius: 0.5rem;
  padding: 0.5rem;
  outline: none;
  border: none;
  background: rgba(0, 0, 0, 0.6);
  -webkit-backdrop-filter: blur(0.5rem);
  backdrop-filter: blur(0.5rem);
  border: 1px solid #fbae3c;
  color: #ffffff;
  transition: all 0.5s ease-out;
}

input[type="text"]:focus,
input[type="email"]:focus,
textarea:focus {
  background: #ffffff;
  color: #333333;
  transition: all 0.5s ease-out;
}

textarea {
  resize: none;
  height: 18.75rem;
}

input[type="button"] {
  width: 6rem;
  border-radius: 0.5rem;
  padding: 0.5rem;
  outline: none;
  border: none;
  background: #ffffff;
  color: #9900ff;
  cursor: pointer;
  border: 1px solid transparent;
  transition: all 0.5s ease-out;
}

input[type="button"]:hover {
  background: rgba(0, 0, 0, 0.6);
  -webkit-backdrop-filter: blur(0.5rem);
  backdrop-filter: blur(0.5rem);
  border: 1px solid #fbae3c;
  color: #ffffff;
  transition: all 0.5s ease-out;
}

::-webkit-input-placeholder {
  color: #ffffff;
}

::-moz-placeholder {
  color: #ffffff;
}

::-ms-placeholder {
  color: #ffffff;
}

::placeholder {
  color: #ffffff;
}

@media only screen and (max-width: 1080px) {
  input[type="text"],
  input[type="email"],
  textarea {
    width: 40vw;
  }
}

@media only screen and (max-width: 768px) {
  .wrap {
    padding: 3rem 0 5rem 0;
  }

  .contact {
    display: block;
    height: auto;
  }

  h1 {
    font-size: 1.8em;
  }

  input[type="text"],
  input[type="email"],
  textarea {
    width: calc(100% - 2.5rem);
  }
}
</style>
