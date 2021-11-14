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
  width: 200px;
  height: 5px;
  border-radius: 10px;
  background: #333333;
  display: inline-block;
  margin: 10px;
}

.value {
  height: 5px;
  background: #9900ff;
  background: linear-gradient(
    90deg,
    rgba(153, 0, 255, 1) 0%,
    rgba(86, 0, 144, 1) 35%,
    rgba(251, 174, 60, 1) 100%
  );

  border-radius: 10px;
}

[data-aos="progress-animate"] {
  width: 0;
  transition-property: width;
}

[data-aos="progress-animate"].aos-animate {
  width: var(--value);
}
</style>
