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
            <div class="textnumber3">50 000 ₽</div>
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
    <div class="row q-gutter-md">
    <q-card
      class="my-card text-white"
      style="background: radial-gradient(circle, #35a2ff 0%, #014a88 100%)"
    >
      <q-card-section
        style="width: 500px"
        class="card">
        <div class="text-h6">СДЕЛКИ ПО МЕНЕДЖЕРАМ</div>
        <div class="textnumber">3516</div>
        <div class="textnumber3">50 000 ₽</div>
        <div style='width: 50%;'>
          <hr>
        </div>
        <div class="row">
          <div class="textnumber6">Admin CRM</div>
          <div style="font-weight: bold">3055 сделок</div>
          <div
            style="opacity: 0.3"
            class="textnumber3">(50 000 ₽)</div>
          <div class="textnumber6">Иван Седых</div>
          <div style="font-weight: bold">151 сделок</div>
          <div
            style="opacity: 0.3"
            class="textnumber3">(50 000 ₽)</div>
        </div>
      </q-card-section>
    </q-card>
  </div>
  </div>



  <div class="row justify-center">
    <q-card bordered class="bg-dark text-white my-card">
      <q-card-section style="background: radial-gradient(circle, #35a2ff 0%, #014a88 100%)">
        <div class="text-h5">ВХОДЯЩИЕ ЗВОНКИ</div>
        <div class="text-number1">5</div>
        <div class="text-subtitle3">за неделю</div>
      </q-card-section>
    </q-card>
    <q-card
      style="background: radial-gradient(circle, #35a2ff 0%, #014a88 100%)"
      class="bg-dark text-white my-card">
      <q-card-section style="background: radial-gradient(circle, #35a2ff 0%, #014a88 100%)">
        <div class="text-h5">ИСХОДЯЩИЕ ЗВОНКИ</div>
        <div class="text-number2">5</div>
        <div class="text-subtitle4">за неделю</div>
      </q-card-section>
    </q-card>
    <q-card
      style="background: radial-gradient(circle, #35a2ff 0%, #014a88 100%)"
      class="bg-dark text-white my-card">
      <q-card-section style="background: radial-gradient(circle, #35a2ff 0%, #014a88 100%)">
        <div class="text-h5">ПРИМЕЧАНИЙ</div>
        <div class="text-number3">5</div>
        <div class="text-subtitle3">за неделю</div>
      </q-card-section>
    </q-card>

    <q-card   class="bg-dark text-white my-card">
      <q-card-section style="background: radial-gradient(circle, #35a2ff 0%, #014a88 100%)">
        <div class="text-h5">УСПЕШНЫЕ СДЕЛКИ</div>
        <div class="text-number4">3082</div>
        <div class="text-subtitle4"></div>
        <div style="font-size:25px">0р</div>
        <div style="width: 50%;">
          <hr>
        </div>
        <div  class="text-number10 "  style="font-size: 30px">+10</div>
        <div class="text-subtitle1">за неделю</div>
      </q-card-section>
    </q-card>

    <q-card flat  class="my-card">
      <q-card-section>
      </q-card-section>
      <q-card>




      </q-card>







    </q-card>
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
        fontSize: '8px',

        fontWeight: 600,
        formatter: function(seriesName, opts) {
          return seriesName + ":  " + opts.w.globals.series[opts.seriesIndex]
        },
      },
    }
  },
  colors: ['blue', 'blue'],
  labels  : ['ИНТЕГРАЦИИ С САЙТОМ ВДЕЛО', 'ВИРТУАЛЬНАЯ АТС МЕГАФОН'],
  responsive: [{
    breakpoint: 200,
    options: {
      legend: {
        show: false
      }
    }
  }]
})
</script>

<style scoped>
.text-number10 {
  font-size: 32px;
  font-weight: bold;
  flex-grow: revert;
  opacity: 0.5;
  color:limegreen
}
.text-number4 {
  opacity: 0.5;

}
.text-number3 {
  opacity: 0.5;

}
.text-number2 {
  opacity: 0.5;
}
.text-number1 {
  opacity: 0.5;

}
.bg-dark {
  font-size: 40px;
  color: limegreen;
  margin-top: 60px;
  width: 320px;
  margin-right: 10px;
  align-items: center;


}
.div {
    opacity: 0.5 ;
  }
.text-h6 {
  font-weight: bold;
  font-size: 10pt;
}

.text-h5 {
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
