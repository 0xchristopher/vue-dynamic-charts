# vue-dynamic-charts

A Vue component library for creating dynamic and responsive charts easily.

## Installation

```bash
npm install vue-dynamic-charts
```

## Usage

Import and register the chart components you need:

```javascript
import Vue from 'vue';
import { BarChart } from 'vue-dynamic-charts';

Vue.component('BarChart', BarChart);
```

Then, you can use them in your templates:

```vue
<template>
  <div>
    <BarChart :data="chartData" :options="chartOptions"></BarChart>
  </div>
</template>

<script>
export default {
  data() {
    return {
      chartData: {...}, // Your chart.js data object
      chartOptions: {...} // Your chart.js options object
    };
  },
};
</script>
```

Replace `BarChart` with `LineChart` or `PieChart` as needed.

## Contributing

We welcome contributions! Please submit pull requests for bug fixes, features, or documentation improvements.
