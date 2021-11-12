<template>
  <div class="wrap">
    <div class="contact">
      <div class="head">
        <h1>Contact Me</h1>
        <div class="social">
          <p><img src="../assets/github.svg" alt="github" /></p>
          <p><img src="../assets/linkedin.svg" alt="linkedin" /></p>
          <p><img src="../assets/twitter.svg" alt="twitter" /></p>
        </div>
      </div>
      <div class="form">
        <input type="email" placeholder="Email" />
        <input type="text" placeholder="Subject" />
        <textarea placeholder="Description"></textarea>
        <input type="button" value="Send" />
      </div>
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
  height: 100vh;
}

.contact {
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

p {
  display: inline-block;
  cursor: pointer;
  padding: 10px;
}

h1 {
  font-size: 3.2em;
  margin-bottom: 10px;
  text-shadow: 0 0 15px #d4d3b8;
}

input,
textarea {
  display: block;
  margin: 20px;
}

input[type="text"],
input[type="email"],
textarea {
  width: 30vw;
  height: 50px;
  border-radius: 10px;
  padding: 10px;
  outline: none;
  border: none;
  background: rgba(0, 0, 0, 0.3);
  -webkit-backdrop-filter: blur(10px);
  backdrop-filter: blur(10px);
  border: 0.1px solid #ffffff;
  color: #ffffff;
}

input[type="text"]:focus,
input[type="email"]:focus,
textarea:focus {
  background: #ffffff;
  color: #333333;
}

textarea {
  resize: none;
  height: 300px;
}

input[type="button"] {
  width: 100px;
  border-radius: 10px;
  padding: 10px;
  outline: none;
  border: none;
  background: #ffffff;
  color: #9900ff;
  cursor: pointer;
  border: 0.1px solid transparent;
}

input[type="button"]:hover {
  background: rgba(0, 0, 0, 0.3);
  -webkit-backdrop-filter: blur(10px);
  backdrop-filter: blur(10px);
  border: 0.1px solid #ffffff;
  color: #ffffff;
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
    padding: 50px 0;
    height: auto;
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
    width: calc(100% - 40px);
  }
}
</style>
