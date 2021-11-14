<template>
  <div class="progress" :style="{ '--value': value * 2 + 'px' }">
    <div class="bar">
      <p
        class="value"
        data-aos="progress-animate"
        data-aos-duration="1000"
        data-aos-easing="ease-out"
      ></p>
    </div>
    <span>{{ value }}%</span>
  </div>
</template>

<script>
export default {
  name: "ProgressBar",

  props: {
    value: String,
  },
};
</script>

<style scoped>
.progress {
  display: grid;
  grid-template-columns: auto auto;
  width: fit-content;
}

.bar {
  width: 12.5rem;
  height: 0.25rem;
  border-radius: 0.5rem;
  background: #333333;
  display: inline-block;
  margin: 0.5rem;
}

.value {
  height: 0.25rem;
  background: #9900ff;
  background: linear-gradient(
    90deg,
    rgba(153, 0, 255, 1) 0%,
    rgba(86, 0, 144, 1) 35%,
    rgba(251, 174, 60, 1) 100%
  );

  border-radius: 0.5rem;
}

[data-aos="progress-animate"] {
  width: 0;
  transition-property: width;
}

[data-aos="progress-animate"].aos-animate {
  width: var(--value);
}

@media only screen and (max-width: 768px) {
  .bar {
    width: 10.9375rem;
  }

  [data-aos="progress-animate"] {
    width: 0;
    transition-property: width;
  }

  [data-aos="progress-animate"].aos-animate {
    width: calc(calc(var(--value) / 8) * 7);
  }

  span {
    font-size: 0.8em;
  }
}
</style>
