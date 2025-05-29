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
            <apexchart type="radialBar"  width='325' :options="options3" :series="series3"/>
          </div>
        </q-card-section>
      </q-card>
    </div>
  </div>
  <div class="row justify-center">
    <q-card bordered class="bg-dark text-white my-card">
      <q-card-section>
        <div class="text-h5">Входящие звонки</div>
        <div class="text-number1">5</div>
        <div class="text-subtitle3">за неделю</div>
      </q-card-section>
    </q-card>
    <q-card class="bg-dark text-white my-card">
      <q-card-section>
        <div class="text-h5">исходящие звонки</div>
        <div class="text-number2">5</div>
        <div class="text-subtitle4">за неделю</div>
      </q-card-section>
    </q-card>
    <q-card class="bg-dark text-white my-card">
      <q-card-section>
        <div class="text-h5">примечаний</div>
        <div class="text-number3">5</div>
        <div class="text-subtitle3">за неделю</div>
      </q-card-section>
    </q-card>

    <q-card   class="bg-dark text-white my-card">
      <q-card-section>

        <div class="text-h5">успешные сделки</div>
        <div class="text-number4">3  082</div>
        <div class="text-subtitle4"></div>
        <div style="font-size:25px">0 р</div>
        <div style="width: 50%;">
          <hr>
        </div>
        <div  class="text-number1 "  style="font-size: 30px">+10</div>
        <div class="text-subtitle1">за неделю</div>
      </q-card-section>
    </q-card>
    <q-card style="background: #1D1D1D" class="bg-dark1 text-white my-card">
      <q-card-section>
      <div>
        <div class="text-h5">исходящие сообщения по менеджерам</div>
        <div style="display:flex;justify-content: flex-end;"class="text-number42" >0</div>
        <div
          style="display:flex;justify-content: flex-end;"
          class="text-subtitle1">за неделю</div>
      </div>
        <div style="width: 20%">
<hr>

  </div>




        </q-card-section>
    </q-card>

    <q-card-section>
      <apexchart type="line"          width='1000' height="500" :options="options3" :series="series3"/>
    </q-card-section>








    <q-card style="background: #1D1D1D" class="bg-dark1 text-white my-card">
      <q-card-section>
        <div class="text-h5">Обработанные беседы</div>
        <div style="display:flex;justify-content: flex-end;" class="text-number42" >0</div>
        <div
          style="display:flex;justify-content: flex-end;"
          class="text-subtitle1">за неделю
        </div>
        <div style="width: 20%">
          <hr>

        </div>
      </q-card-section>
    </q-card>




        <q-card style="background: #1D1D1D" class="bg-dark1 text-white my-card">
          <q-card-section>
            <div>
            <div class="text-h5">Входящиесообщения</div>
            <div style="display:flex;justify-content: flex-end;" class="text-number42" >0</div>
            <div
              style="display:flex;justify-content: flex-end;"
              class="text-subtitle1">за неделю
            </div>
            <div style="width: 20%">
              <hr style="opacity: 5%; height: auto">
            </div>
            </div>
          </q-card-section>
        </q-card>
    <q-card style="background: #1D1D1D" class="bg-dark1 text-white my-card">
      <q-card-section>
        <div>
          <div class="text-h5">Среднее время ответа</div>
          <div style="width: 20%">
          </div>
        </div>
      </q-card-section>
    </q-card>

  </div>
  <q-card style="background: #1D1D1D; height: auto;" class="bg-dark1 text-white my-card">
    <q-card-section>
      <div>
        <div class="text-h5">индекс потребительской лояльности(NPS)</div>
        </div>
        <div style="width: 20%">
          <hr style="opacity: 5%">
        </div>

      <apexchart type="radialBar" height="350" :options="options4" :series="series4"></apexchart>
      <div>
      <div class="text-h5" style="opacity: 5%">*NPS позволяет оценить уровень удовлетворенности клиентов Формула расчета: %Сторонников - % Критков</div>
    </div>
    </q-card-section>
  </q-card>
</template>




<script setup>
import { ref } from 'vue';


let options4 = {
    chart: {
      height: 200,
      type: 'radialBar',
    },
    plotOptions: {
      radialBar: {
        hollow: {
          size: '70%',
        }
      },
    },
    labels: ['NPS*'],
  }

let series4 = [70]

// var chart = new ApexCharts(document.querySelector("#chart"), options);
// chart.render();


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




let series3 = ref([{
  name: "Desktops",
  data: [0, 15, 30, ]
}])

let options3= ref({
  chart: {

    background: 'rgba(12,37,61,.95)',
    width: 500,
    height: 500,
    type: 'line',
    zoom: {
      enabled: false
    }
  },
  dataLabels: {
    enabled: false
  },
  stroke: {
    colors: [
      'green'
    ],
    curve: 'straight'
  },
  title: {
    text: 'прогноз продаж',
    align: 'left',
    color: '#666'
  },
  grid: {
    row: {
        colors: ['#f3f3f3', 'transparent'], // takes an array which will be repeated on columns
      opacity: 0.5
    },
  },
  xaxis: {

    categories: ['сделок в работе сейчас', 'по прошествии 5 дней ' ,'  ' ],

  }
})
</script>

<style>
.text-number1 {
  font-size: 32px;
  font-weight: bold;
  flex-grow: revert;
  opacity: 20%;
}
.text-number4 {
  opacity: 20%;
}
.text-number42 {
  opacity: 20%;

}
.text-number3 {
  opacity: 20%;
}
.text-number2 {
  opacity: 20%;
}
.text-number1 {
  opacity: 20%;
}
.bg-dark {
  //line-height: 120px;
  font-size: 40px;

  margin-top: 60px;
  width: 320px;
  margin-right: 10px;
  align-items: center;
}
.bg-dark1 {
  //line-height: 120px;
  font-size: 40px;

  margin-top: 60px;
  width: 500px;
  height: 500px;
  margin-right: 10px;
  align-items: center;
}
.div {
    opacity: 20% ;
  }
.text-h6 {
  font-weight: bold;
  font-size: 10pt;
}

.text-subtitle2 {
  font-size: 10pt;
}
.text-subtitle1 {
  font-size: 10pt;
  opacity: 50%;
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

.apexcharts-grid-row {
  fill: rgba(12,37,61,.95);
}
</style>
