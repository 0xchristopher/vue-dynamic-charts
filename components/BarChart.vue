<template>
  <div class="chart-container">
    <canvas ref="canvas"></canvas>
  </div>
</template>

<script>
import { Chart } from 'chart.js';

export default {
  name: 'BarChart',
  props: ['data', 'options'],
  mounted() {
    new Chart(this.$refs.canvas, {
      type: 'bar',
      data: this.data,
      options: this.options,
    });
  },
};
</script>

<style scoped>
.chart-container {
  position: relative;
  width: 100%;
  height: 400px;
}
</style>
