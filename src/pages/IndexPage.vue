<template>
  <q-page class="flex flex-center">
    <apexchart type="bar" height="350" width='500' :options="options" :series="series"/>
    <apexchart type="donut"  width='500' :options="options2" :series="series2"/>
  </q-page>

</template>

<script setup>
import {ref } from 'vue';


let series = ref([
  {
    name: 'test',
    data: [ 30, 40,50,43,65,84,14,98,35]
  }
  ]
)

let options= ref({ xaxis: { categories: ['test1', 'test2', 'test3','test4','test5','test6','test7','test8','test9',]}})

let series2 = ref([50, 23, 11, 99, 48])

let options2 = ref({
  chart: {
    type: 'donut',
  },
  labels: ['test-1','test-2','test-3','test-4','test-5',],
  responsive: [{
    breakpoint: 480,
    options: {
      chart: {
        width: 500
      },
      legend: {
        position: 'bottom'
      }
    }
  }],
  colors: ['orange', 'green', 'blue', 'red', 'purple'],
  dataLabels: {
    enabled: true
  },
  legend: {
    position: 'right',
    offsetY: 0,
    height: 230,
  }
}
)
</script>
