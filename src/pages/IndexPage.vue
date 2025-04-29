<template>
  <div class="row q-gutter-md">
    <div>
      <div class="row q-gutter-md">
        <q-card
          class="my-card text-white"
          style="background: radial-gradient(circle, #35a2ff 0%, #014a88 100%)"
        >
          <q-card-section class="card">
            <div class="text-h6">ПРОСРОЧЕННЫЕ ЗАДАЧИ</div>
            <div class="textnumber">65</div>
            <div style="width: 50%;">
                 <hr>
            </div>
            <div class="textnumber2">0</div>
            <div class="text-subtitle2">за неделю</div>
          </q-card-section>
        </q-card>
        <q-card
          class="my-card text-white"
          style="background: radial-gradient(circle, #35a2ff 0%, #014a88 100%)"
        >
          <q-card-section class="card">
            <div class="text-h6">ВЫПОЛНЕННЫЕ ЗАДАЧИ</div>
            <div class="textnumber">0</div>
            <div class="text-subtitle2">за неделю</div>
          </q-card-section>
        </q-card>
      </div>
      <div class="row q-gutter-md">
      <q-card
        class="my-card text-white"
        style="background: radial-gradient(circle, #35a2ff 0%, #014a88 100%)"
      >
        <q-card-section class="card">
          <div class="text-h6">ЗАДАЧИ К ВЫПОЛНЕНИЮ</div>
          <div class="textnumber">75</div>
          <div style="width: 50%;">
            <hr>
          </div>
          <div class="textnumber2">+8</div>
          <div class="text-subtitle2">за неделю</div>
        </q-card-section>
      </q-card>
      <q-card
        class="my-card text-white"
        style="background: radial-gradient(circle, #35a2ff 0%, #014a88 100%)"
      >
        <q-card-section class="card">
          <div class="text-h6">СДЕЛОК БЕЗ ЗАДАЧ</div>
          <div class="textnumber">3506</div>
          <div class="textnumber3">50 000р</div>
          <div style="width: 50%;">
            <hr>
          </div>
          <div class="textnumber2">+8</div>
          <div class="text-subtitle2">за неделю</div>
        </q-card-section>
      </q-card>
    </div>
    </div>
    <div class="row q-gutter-md">
      <q-card
        class="my-card text-white"
        style="background: radial-gradient(circle, #35a2ff 0%, #014a88 100%)"
      >

    <q-card-section class="card">
      <div class="text-h6">ИСТОЧНИКИ СДЕЛОК</div>
      <div class="flex flex-center">
        <apexchart type="radialBar"  width='325' :options="options2" :series="series2"/>
      </div>
    </q-card-section>
      </q-card>
    </div>
  </div>





</template>




<script setup>

import { ref } from 'vue';




let series2 = ref([100,100])

let options2= ref({
  chart: {
    height: 390,
    type: 'radialBar',
  },
  plotOptions: {
    radialBar: {
      offsetY: 0,
      startAngle: 0,
      endAngle: 270,
      hollow: {
        margin: 5,
        size: '30%',
        background: 'transparent',
        image: undefined,
      },
      dataLabels: {
        name: {
          show: false,
        },
        value: {
          show: false,
        }
      },
      barLabels: {
        enabled: true,
        useSeriesColors: true,
        offsetX: -8,
        fontSize: '16px',
        formatter: function(seriesName, opts) {
          return seriesName + ":  " + opts.w.globals.series[opts.seriesIndex]
        },
      },
    }
  },
  colors: ['#0084ff', '#0084ff'],
  labels  : ['ИНТЕГРАЦИИ С САЙТОМ ВДЕЛО', 'ВИРТУАЛЬНАЯ АТС МЕГАФОН'],
  responsive: [{
    breakpoint: 480,
    options: {
      legend: {
        show: false
      }
    }
  }]
})

</script>



<style scoped>
.text-h6 {
  font-weight: bold;
  font-size: 10pt;
}

.text-subtitle2 {
  font-size: 10pt;
}

.textnumber {
  font-size: 20pt;
  opacity: 0.5;
}

.textnumber2 {
  color:limegreen;
  opacity: 0.5;
}

.textnumber3 {
  font-size: 10pt;
}

.card {
}
</style>
