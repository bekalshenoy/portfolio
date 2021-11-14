<template>
  <div class="wrap">
    <div class="nav-bar">
      <div
        class="menu"
        data-aos="fade-down"
        data-aos-duration="1000"
        data-aos-easing="ease-out"
      >
        <div
          :class="
            innerWidth <= 768
              ? showMenu
                ? 'menu-bars open'
                : 'menu-bars'
              : 'menu-bars'
          "
          @click="toggleMenu"
        >
          <span></span>
          <span></span>
          <span></span>
        </div>
      </div>
      <div
        :class="innerWidth <= 768 ? (showMenu ? 'nav slide' : 'nav') : 'nav'"
        :style="
          innerWidth <= 768
            ? showMenu
              ? 'display: block;height: 450px;visibility: visible;transition: all 0.5s ease-out;'
              : 'height: 0;transition:all 0.5s ease-out;'
            : ''
        "
        :data-aos="innerWidth <= 768 ? null : 'fade-right'"
        :ata-aos-duration="innerWidth <= 768 ? null : '1000'"
        :data-aos-easing="innerWidth <= 768 ? null : 'ease-out'"
      >
        <a href="#about">About</a>
        <a href="#experience">Experience</a>
        <a href="#skills">Skills</a>
        <a href="#projects">Projects</a>
        <a href="#education">Education</a>
        <a href="#volunteering">Volunteering</a>
        <a href="#contact">Contact</a>
      </div>
      <div
        class="social"
        data-aos="fade-left"
        data-aos-duration="1000"
        data-aos-easing="ease-out"
      >
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
  </div>
</template>

<script>
export default {
  name: "NavBar",

  data() {
    return {
      showMenu: false,
      innerWidth: window.innerWidth,
    };
  },

  mounted() {
    window.addEventListener("resize", () => {
      this.innerWidth = window.innerWidth;
    });
  },

  methods: {
    toggleMenu() {
      this.showMenu = !this.showMenu;
    },
  },

  watch: {
    innerWidth(val) {
      if (val > 768 && this.showMenu) this.showMenu = false;
    },
  },
};
</script>

<style scoped>
.wrap {
  position: fixed;
  width: 100%;
  z-index: 2;
}

.nav-bar {
  width: 100%;
  max-width: 1920px;
  margin: 0 auto;
  color: #ffffff;
}

.nav,
.social {
  height: 50px;
  background: rgba(0, 0, 0, 0.6);
  border: 1px solid #fbae3c;
  -webkit-backdrop-filter: blur(10px);
  backdrop-filter: blur(10px);
  border-radius: 50px;
  padding: 0 10px;
  margin: 10px;
}

.nav {
  position: absolute;
  left: 0;
}

.social {
  position: absolute;
  right: 0;
}

a {
  text-decoration: none;
  display: inline-block;
  cursor: pointer;
  padding: 10px;
  transition: all 0.5s ease-out;
  color: #ffffff;
}

.nav a:hover {
  color: #9900ff;
  transition: all 0.5s ease-out;
}

.social a:hover {
  opacity: 0.8;
  transition: all 0.5s ease-out;
}

.social img {
  height: 30px;
  width: 30px;
}

/* Hamburger */
.menu {
  background: rgba(0, 0, 0, 0.6);
  border: 1px solid #fbae3c;
  -webkit-backdrop-filter: blur(10px);
  backdrop-filter: blur(10px);
  border-radius: 50px;
  padding: 10px;
  display: none;
  position: fixed;
  left: calc(50% - 20px);
  top: 20px;
  text-align: center;
}

.menu-bars {
  display: flex;
  flex-direction: column;
  height: 1.25em;
  justify-content: space-between;
  position: relative;
}

.menu-bars span {
  display: block;
  width: 1.75em;
  height: 0.1875em;
  z-index: 2;
  background-color: #ffffff;
  border-radius: 0.1875em;
  transition: all 0.3s;
}

.menu-bars span:nth-child(1) {
  transform-origin: 0 0;
}

.menu-bars span:nth-child(3) {
  transform-origin: 0 100%;
}

.open span {
  width: 1.75em;
}

.open span:nth-child(1) {
  transform: rotate(33deg) translate(3px, -1px);
}

.open span:nth-child(3) {
  transform: rotate(-33deg) translate(3px, 0);
}

.open span:nth-child(2) {
  opacity: 0;
  transform: scale(0);
}

.slide a {
  opacity: 0;
}

@media only screen and (max-width: 1080px) {
  .social {
    display: none;
  }
}

@media only screen and (max-width: 768px) {
  .menu {
    display: block;
  }

  .nav {
    visibility: hidden;
  }

  .nav a {
    visibility: hidden;
    opacity: 0;
  }

  a {
    padding: 20px;
  }

  .nav {
    width: 200px;
    position: fixed;
    left: calc(50% - 100px);
    top: 80px;
    text-align: center;
    border-radius: 20px;
    margin: 0;
  }

  .slide a {
    visibility: visible;
    opacity: 1;
    transition: opacity 0.5s ease-out 0.5s;
  }
}
</style>
