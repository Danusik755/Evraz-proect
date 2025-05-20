<template>
  <div class="row justify-center items-start q-gutter-md">
    <q-card
      class="my-card text-white"
      style="background:rgba(12, 37, 61, .95)"
    >
      <q-card-section
        style="height:175px"

        class="card">
        <div class="text-h6">ПРОСРОЧЕННЫЕ ЗАДАЧИ</div>
        <div class="textnumber">65</div>
        <div
          style="width: 50%;">
          <hr>
        </div>
        <div class="textnumber2">0</div>
        <div class="text-subtitle2">за неделю</div>
      </q-card-section>
    </q-card>
    <q-card
      class="my-card text-white"
      style="background: rgba(12, 37, 61, .95)"
    >
      <q-card-section
        style="height:175px"
        class="card">
        <div class="text-h6">ВЫПОЛНЕННЫЕ ЗАДАЧИ</div>
        <div class="textnumber">0</div>
        <div class="text-subtitle2">за неделю</div>
      </q-card-section>
    </q-card>
    <q-card
      class="my-card text-white"
      style="background: rgba(12, 37, 61, .95)"
    >
      <q-card-section
        style="height:175px"
        class="card">
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
      style="background: rgba(12, 37, 61, .95)"
    >
      <q-card-section
        style="height:175px"
        class="card">
        <div class="text-h6">СДЕЛОК БЕЗ ЗАДАЧ</div>
        <div class="textnumber">3506</div>
        <div
          style="font-weight: bold"
          class="textnumber11">50 000 ₽
        </div>
        <div style="width: 50%;">
          <hr>
        </div>
        <div class="textnumber2">+8</div>
        <div class="text-subtitle2">за неделю</div>
      </q-card-section>
    </q-card>
    <q-card
      class="my-card text-white"
      style="background: rgba(12, 37, 61, .95)"
    >

      <q-card-section class="card">
        <div class="text-h6">ИСТОЧНИКИ СДЕЛОК</div>
        <div class="flex flex-center">
          <apexchart type="radialBar" width='325' :options="options2" :series="series2"/>
        </div>
      </q-card-section>
    </q-card>
    <q-card
      class="my-card text-white"
      style="background: rgba(12, 37, 61, .95)"
    >
      <q-card-section
        style="width: 500px"
        class="card">
        <div class="text-h6">СДЕЛКИ ПО МЕНЕДЖЕРАМ</div>
        <div class="textnumber">3516</div>
        <div class="row justify-center items-start q-gutter-md">
          <div
            style="margin-left: 375px"
            class="textnumber2">+8
          </div>
          <div class="row-q-gutter-xs">за неделю</div>
        </div>
        <div
          style="font-weight: bold"
          class="textnumber11">50 000 ₽
        </div>
        <div style='width: 50%;'>
          <hr>
        </div>
        <div
          style="margin-bottom: 10px"
          class="row q-gutter-xs">
          <div class="textnumber6">Admin CRM</div>
          <div style="font-weight: bold">3055 сделок</div>
          <div
            style="opacity: 0.3"
            class="textnumber3">(50 000 ₽)
          </div>
          <div
            class="textnumber2"
            style="margin-left: 220px">+6</div>
          <q-linear-progress :value="1" color="yellow" class="line"></q-linear-progress>
        </div>
        <div
          style="margin-bottom: 10px"
          class="row q-gutter-xs">
          <div class="textnumber6">Иван Седых</div>
          <div style="font-weight: bold"> 151 сделок</div>
          <div
            style="opacity: 0.3"
            class="textnumber3">(0 ₽)
          </div>
          <div
            class="textnumber2"
            style="margin-left: 263px">0</div>
          <q-linear-progress :value="0.04" color="yellow" class="line"></q-linear-progress>
        </div>
        <div
          style="margin-bottom: 10px"
          class="row q-gutter-xs">
          <div class="textnumber6">Александр Михайлов</div>
          <div style="font-weight: bold"> 146 сделок</div>
          <div
            style="opacity: 0.3"
            class="textnumber3">(0 ₽)
          </div>
          <div
            class="textnumber2"
            style="margin-left: 196px">+2</div>
          <q-linear-progress :value="0.04" color="yellow" class="line"></q-linear-progress>
        </div>
        <div
          style="margin-bottom: 10px"
          class="row q-gutter-xs">
          <div class="textnumber6">Ксения Евдокимова</div>
          <div style="font-weight: bold"> 89 сделок</div>
          <div
            style="opacity: 0.3"
            class="textnumber3">(0 ₽)
          </div>
          <div
            class="textnumber2"
            style="margin-left: 220px">0</div>
          <q-linear-progress :value="0.02" color="yellow" class="line"></q-linear-progress>
        </div>
        <div
          style="margin-bottom: 10px"
          class="row q-gutter-xs">
          <div class="textnumber6">Елизавета Ткачева</div>
          <div style="font-weight: bold"> 43 сделок</div>
          <div
            style="opacity: 0.3"
            class="textnumber3">(0 ₽)
          </div>
          <div
            class="textnumber2"
            style="margin-left: 224px">0</div>
          <q-linear-progress :value="0.01" color="yellow" class="line"></q-linear-progress>
        </div>
        <div
          style="margin-bottom: 10px"
          class="row q-gutter-xs  ">
          <div class="textnumber6">Другие</div>
          <div style="font-weight: bold"> 32 сделок</div>
          <div
            style="opacity: 0.3"
            class="textnumber3">(0 ₽)
          </div>
          <div
            class="textnumber2"
            style="margin-left: 303px">0</div>
          <q-linear-progress :value="0.008" color="yellow" class="line"></q-linear-progress>
        </div>
      </q-card-section>
    </q-card>
    <q-card
      class="my-card text-white"
      style="background: rgba(12, 37, 61, .95)"
    >
      <q-card-section
        style="width: 400px"
        class="card">
        <div class="text-h6">ЦЕЛИ</div>
        <div class="flex flex-center">
          <apexchart type="radialBar" width='325' :options="options3" :series="series3"/>
        </div>
      </q-card-section>
    </q-card>
    <q-card
      class="my-card text-white"
      style="background: rgba(12, 37, 61, .95)"
    >
      <q-card-section
        style="width: 400px"
        class="card">
        <div
          class="text-h6">ИСПОЛЬЗОВАНИЕ СИСТЕМЫ ЗА НЕДЕЛЮ
        </div>
        <div
          style="display: flex; justify-content: flex-end"
          class="textnumber20">За неделю
        </div>
        <div
          style="margin-top: 20px"
          class="row q-gutter-xs">
          <img
            style="width:30px"
            src="https://avatars.mds.yandex.net/get-socsnippets/12856884/2a0000019158c1fcb75dc89d8e6c6fec8753/square_83">
          <div>Admin CRM</div>
          <div
            style="font-weight: bold"
            class="row q-gutter-xs"></div>
          <div style="font-weight: bold">0 м.</div>
          <div
            class="text11">18 м.
          </div>
          <q-linear-progress :value="0" color="yellow" class="line"></q-linear-progress>
          <img
            style="width:30px"
            src="https://avatars.mds.yandex.net/i?id=9f64755eec4927fe8ba29cbd5d1a3749d82fcdae-3590262-images-thumbs&n=13">
          <div class="row q-gutter-xs">Валерий Богинский</div>
          <div
            style="font-weight: bold"
            class="row q-gutter-xs">0 м.
          </div>
          <div
            class="text12">10 м.
          </div>
          <q-linear-progress :value="0" color="black" class="line"></q-linear-progress>
        </div>
      </q-card-section>
    </q-card>
    <q-card
      class="my-card text-white"
      style="background: rgba(12, 37, 61, .95)"
    >
      <q-card-section
        style="width: 400px"
        class="row-q-gutter-xs">
        <div class="text-h6">ПОСЛЕДНИЕ ФАЙЛЫ</div>
        <div class="row q-mb-md">
          <img
            style="width: 50px"
            src="https://avatars.mds.yandex.net/i?id=85e05f3c027cadf9e1d8a614850ed524a9a8bd66-9068341-images-thumbs&n=13"
            class="q-mr-sm"
          >
          Доходы "ЕВРАЗ"
        </div>
        <div
          style="font-weight: bold"
          class="row q-gutter-xs">
        </div>

        <div class="row q-mb-md">
          <img
            style="width: 50px"
            src="https://avatars.mds.yandex.net/i?id=85e05f3c027cadf9e1d8a614850ed524a9a8bd66-9068341-images-thumbs&n=13"
            class="q-mr-sm"
          >
          Задачи "ЕВРАЗ"
        </div>
        <div
          style="font-weight: bold"
          class="row q-gutter-xs">
        </div>

        <div class="row q-mb-md">
          <img
            style="width: 50px"
            src="https://avatars.mds.yandex.net/i?id=85e05f3c027cadf9e1d8a614850ed524a9a8bd66-9068341-images-thumbs&n=13"
            class="q-mr-sm">
          Работники "ЕВРАЗ"
        </div>
        <div
          style="font-weight: bold"
          class="row q-gutter-xs"></div>

        <div class="row q-mb-md">
          <img
            style="width: 50px"
            src="https://avatars.mds.yandex.net/i?id=85e05f3c027cadf9e1d8a614850ed524a9a8bd66-9068341-images-thumbs&n=13"
            class="q-mr-sm"
          >
          Важная информация "ЕВРАЗ"
        </div>
        <div
          style="font-weight: bold"
          class="row q-gutter-xs"></div>

        <div class="row q-mb-md">
          <img
            style="width: 50px"
            src="https://avatars.mds.yandex.net/i?id=85e05f3c027cadf9e1d8a614850ed524a9a8bd66-9068341-images-thumbs&n=13"
            class="q-mr-sm"
          >
          Секреты "ЕВРАЗ"
        </div>
        <div
          style="font-weight: bold"
          class="row q-gutter-xs"></div>

        <div class="row q-mb-md">
          <img
            style="width: 50px"
            src="https://avatars.mds.yandex.net/i?id=85e05f3c027cadf9e1d8a614850ed524a9a8bd66-9068341-images-thumbs&n=13"
            class="q-mr-sm"
          >
          База данных "ЕВРАЗ"
        </div>
        <div
          style="font-weight: bold"
          class="row q-gutter-xs">
        </div>
      </q-card-section>
    </q-card>
    <q-card bordered class="bg-dark text-white my-card">
      <q-card-section style="background: rgba(12, 37, 61, .95)">
        <div class="text-h5">ВХОДЯЩИЕ ЗВОНКИ</div>
        <div class="text-number1">5</div>
        <div class="text-subtitle3">за неделю</div>
      </q-card-section>
    </q-card>
    <q-card
      style="background: rgba(12, 37, 61, .95)"
      class="bg-dark text-white my-card">
      <q-card-section style="background: rgba(12, 37, 61, .95)">
        <div class="text-h5">ИСХОДЯЩИЕ ЗВОНКИ</div>
        <div class="text-number2">5</div>
        <div class="text-subtitle4">за неделю</div>
      </q-card-section>
    </q-card>
    <q-card
      style="background: rgba(12, 37, 61, .95)"
      class="bg-dark text-white my-card">
      <q-card-section style="background: rgba(12, 37, 61, .95)">
        <div class="text-h5">ПРИМЕЧАНИЙ</div>
        <div class="text-number3">5</div>
        <div class="text-subtitle3">за неделю</div>
      </q-card-section>
    </q-card>

    <q-card class="bg-dark text-white my-card">
      <q-card-section style="background: rgba(12, 37, 61, .95)">
        <div class="text-h5">УСПЕШНЫЕ СДЕЛКИ</div>
        <div class="text-number4">3082</div>
        <div class="text-subtitle4"></div>
        <div style="font-size:25px">0р</div>
        <div style="width: 50%;">
          <hr>
        </div>
        <div class="text-number10 " style="font-size: 30px">+10</div>
        <div class="text-subtitle1">за неделю</div>
      </q-card-section>
    </q-card>


    <q-card flat class="my-card">
      <q-card-section>
      </q-card-section>
      <q-card>


      </q-card>


    </q-card>
  </div>
</template>


<script setup>
import {ref} from 'vue';


let series2 = ref([100, 100])

let options2 = ref({
  chart: {
    width: 390,
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
        formatter: function (seriesName, opts) {
          return seriesName + ":  " + opts.w.globals.series[opts.seriesIndex]
        },
      },
    }
  },
  colors: ['#35a2ff', '#35a2ff'],
  labels: ['ИНТЕГРАЦИИ С САЙТОМ ВДЕЛО', 'ВИРТУАЛЬНАЯ АТС МЕГАФОН'],
  responsive: [{
    breakpoint: 200,
    options: {
      legend: {
        show: false
      }
    }
  }]
})

let series3 = ref([100, 100, 100, 100, 100])

let options3 = ref({
  chart: {
    width: 390,
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
        formatter: function (seriesName, opts) {
          return seriesName + ":  " + opts.w.globals.series[opts.seriesIndex]
        },
      },
    }
  },
  colors: ['#35a2ff', '#35a2ff'],
  labels: ['ИНТЕГРАЦИИ С САЙТОМ ВДЕЛО', 'ВИРТУАЛЬНАЯ АТС МЕГАФОН'],
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

.text11 {
  color: red;
  margin-left: 185px;
}

.text12 {
  color: red;
  margin-left: 137px;
}

.line {
  border-radius: 10px;
}

.text-number10 {
  font-size: 32px;
  font-weight: bold;
  flex-grow: revert;
  opacity: 0.5;
  color: limegreen;
}

.text-number4 {
  opacity: 0.5;
  color: mediumpurple;

}

.text-number3 {
  opacity: 0.5;
  color: mediumpurple;
}

.text-number2 {
  opacity: 0.5;
  color: mediumpurple;
}

.text-number1 {
  opacity: 0.5;
  color: mediumpurple;
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
  opacity: 0.5;
  color: mediumpurple;
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
  color: mediumpurple;
}

.textnumber2 {
  color: limegreen;
  opacity: 0.5;
}

.textnumber3 {
  font-size: 10pt;
  color: mediumpurple;
}

.card {
}
</style>
