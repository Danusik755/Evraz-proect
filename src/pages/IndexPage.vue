<template>
  <div class="container">
    <div class="vdelo">
      vdelocrm
    </div>
    <div class="row items-stretch q-col-gutter-md">
      <div class="col-4">
        <div class="flex full-height" style="gap: 16px;">
          <div style="flex: 1;">
            <q-card
              class="my-card text-white full-height"
              style="background:rgba(12, 37, 61, .95);"
            >
              <q-card-section class="card">
                <div class="text-h6">ПРОСРОЧЕННЫЕ ЗАДАЧИ</div>
                <div class="textnumber">52</div>
                <div
                  style="width: 50%;">
                  <hr>
                </div>
                <div class="textnumber2">+2</div>
                <div class="text-subtitle2">за неделю</div>
              </q-card-section>
            </q-card>
          </div>
          <div style="flex: 1;">
            <q-card
              class="my-card text-white full-height"
              style="background: rgba(12, 37, 61, .95);"
            >
              <q-card-section
                class="card">
                <div class="text-h6">ВЫПОЛНЕННЫЕ ЗАДАЧИ</div>
                <div class="textnumber">3</div>
                <div class="text-subtitle2">за неделю</div>
              </q-card-section>
            </q-card>
          </div>
          <div style="flex: 1;">
            <q-card
              class="my-card text-white full-height"
              style="background: rgba(12, 37, 61, .95);"
            >
              <q-card-section
                class="card">
                <div class="text-h6">ЗАДАЧИ К ВЫПОЛНЕНИЮ</div>
                <div class="textnumber">83</div>
                <div style="width: 50%;">
                  <hr>
                </div>
                <div class="textnumber2">+7</div>
                <div class="text-subtitle2">за неделю</div>
              </q-card-section>
            </q-card>
          </div>
          <div style="flex: 1;">
            <q-card
              class="my-card text-white full-width full-height"
              style="background: rgba(12, 37, 61, .95);"
            >
              <q-card-section
                class="card">
                <div class="text-h6">СДЕЛОК БЕЗ ЗАДАЧ</div>
                <div class="textnumber">2894</div>
                <div
                  style="font-weight: bold"
                  class="textnumber11">90 000 ₽
                </div>
                <div style="width: 50%;">
                  <hr>
                </div>
                <div class="textnumber2">+9</div>
                <div class="text-subtitle2">за неделю</div>
              </q-card-section>
            </q-card>
          </div>
        </div>
      </div>
      <div class="col-4">
        <q-card
          class="my-card text-white full-height"
          style="background: rgba(12, 37, 61, .95)"
        >
          <q-card-section class="card">
            <div class="text-h6">ИСТОЧНИКИ СДЕЛОК</div>
            <div class="flex flex-center">
              <apexchart type="radialBar" width='325' :options="options2" :series="series2"/>
            </div>
          </q-card-section>
        </q-card>
      </div>

      <div class="col-4">
        <q-card
          class="my-card text-white full-height"
          style="background: rgba(12, 37, 61, .95)"
        >
          <q-card-section
            class="card">
            <div class="text-h6">СДЕЛКИ ПО МЕНЕДЖЕРАМ</div>
            <div class="row justify-between">
              <div>
                <div class="textnumber">3516</div>
                <div
                  style="font-weight: bold"
                  class="textnumber11">90 000 ₽
                </div>
              </div>

              <div>
                <div
                  class="textnumber2 text-right">+8
                </div>
                <div class="row-q-gutter-xs">за неделю</div>
              </div>
            </div>

            <div style='width: 50%;'>
              <hr>
            </div>
          </q-card-section>

          <q-card-section>
            <div style="margin-bottom: 10px">
              <div class="row justify-between items-center q-mb-xs">
                <div class="row items-center q-gutter-xs">
                  <div class="textnumber6">Admin CRM</div>
                  <div style="font-weight: bold">3055 сделок</div>
                  <div
                    style="opacity: 0.3"
                    class="textnumber3">(90 000 ₽)
                  </div>
                </div>

                <div class="textnumber2">
                  +6
                </div>
              </div>
              <q-linear-progress :value="1" color="yellow" class="line"></q-linear-progress>
            </div>

            <div style="margin-bottom: 10px">
              <div class="row justify-between items-center q-mb-xs">
                <div class="row items-center q-gutter-xs">
                  <div class="textnumber6">Иван Седых</div>
                  <div style="font-weight: bold">151 сделка</div>
                  <div
                    style="opacity: 0.3"
                    class="textnumber3">(0 ₽)
                  </div>
                </div>

                <div class="textnumber2">
                  0
                </div>
              </div>
              <q-linear-progress :value="0.04" color="yellow" class="line"></q-linear-progress>
            </div>

            <div style="margin-bottom: 10px">
              <div class="row justify-between items-center q-mb-xs">
                <div class="row items-center q-gutter-xs">
                  <div class="textnumber6"> Александр Михайлов</div>
                  <div style="font-weight: bold">146 сделок</div>
                  <div
                    style="opacity: 0.3"
                    class="textnumber3">(0 ₽)
                  </div>
                </div>

                <div class="textnumber2">
                  0
                </div>
              </div>
              <q-linear-progress :value="0.04" color="yellow" class="line"></q-linear-progress>

            </div>
            <div style="margin-bottom: 10px">
              <div class="row justify-between items-center q-mb-xs">
                <div class="row items-center q-gutter-xs">
                  <div class="textnumber6"> Ксения Евдокимова</div>
                  <div style="font-weight: bold">89 сделок</div>
                  <div
                    style="opacity: 0.3"
                    class="textnumber3">(0 ₽)
                  </div>
                </div>

                <div class="textnumber2">
                  0
                </div>
              </div>
              <q-linear-progress :value="0.02" color="yellow" class="line"></q-linear-progress>

            </div>
            <div style="margin-bottom: 10px">
              <div class="row justify-between items-center q-mb-xs">
                <div class="row items-center q-gutter-xs">
                  <div class="textnumber6"> Елизавета Ткачева</div>
                  <div style="font-weight: bold">43 сделки</div>
                  <div
                    style="opacity: 0.3"
                    class="textnumber3">(0 ₽)
                  </div>
                </div>

                <div class="textnumber2">
                  0
                </div>
              </div>
              <q-linear-progress :value="0.01" color="yellow" class="line"></q-linear-progress>

            </div>
            <div style="margin-bottom: 10px">
              <div class="row justify-between items-center q-mb-xs">
                <div class="row items-center q-gutter-xs">
                  <div class="textnumber6"> Другие</div>
                  <div style="font-weight: bold">32 сделки</div>
                  <div
                    style="opacity: 0.3"
                    class="textnumber3">(0 ₽)
                  </div>
                </div>

                <div class="textnumber2">
                  0
                </div>
              </div>
              <q-linear-progress :value="0.008" color="yellow" class="line"></q-linear-progress>
            </div>
          </q-card-section>
        </q-card>
      </div>

      <div class="col-4">
        <q-card
          class="my-card text-white "
          style="background: rgba(12, 37, 61, .95)"
        >
          <q-card-section
            style="width: 400px"
            class="card3">
            <div class="text-h6">ЦЕЛИ</div>
            <div class="flex flex-center">
              <apexchart type="donut" height='325' width='340' :options="options5" :series="series5"/>
              <div class="arrow"></div>
            </div>
          </q-card-section>
        </q-card>
      </div>

      <div class="col-4 ">
        <q-card
          class="my-card text-white full-height"
          style="background: rgba(12, 37, 61, .95)"
        >
          <q-card-section
            style="width: 400px"
            class="card4">
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
                class="image"
                style="width:30px"
                src="https://avatars.mds.yandex.net/get-socsnippets/12856884/2a0000019158c1fcb75dc89d8e6c6fec8753/square_83">
              <div>Admin CRM</div>
              <div
                style="font-weight: bold"
                class="row q-gutter-xs"></div>
              <div style="font-weight: bold">7 м.</div>
              <div
                class="text11">28 м.
              </div>
              <q-linear-progress :value="0" color="yellow" class="line"></q-linear-progress>
              <img
                class="img"
                style="width:30px"
                src="https://avatars.mds.yandex.net/i?id=9f64755eec4927fe8ba29cbd5d1a3749d82fcdae-3590262-images-thumbs&n=13">
              <div class="row q-gutter-xs">Валерий Богинский</div>
              <div
                style="font-weight: bold"
                class="row q-gutter-xs">2 м.
              </div>
              <div
                class="text12">13 м.
              </div>
              <q-linear-progress :value="0" color="black" class="line"></q-linear-progress>
            </div>
          </q-card-section>
        </q-card>
      </div>

      <div class="col-4">
        <q-card
          class="my-card text-white full-height"
          style="background: rgba(12, 37, 61, .95)"
        >
          <q-card-section
            style="width: 400px"
            class="row-q-gutter-xs">
            <div class="text-h6">ПОСЛЕДНИЕ ФАЙЛЫ</div>
            <div
              style="font-weight: bold"
              class="row q-mb-md">
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

            <div
              style="font-weight: bold"
              class="row q-mb-md">
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

            <div
              style="font-weight: bold"
              class="row q-mb-md">
              <img
                style="width: 50px"
                src="https://avatars.mds.yandex.net/i?id=85e05f3c027cadf9e1d8a614850ed524a9a8bd66-9068341-images-thumbs&n=13"
                class="q-mr-sm">
              Работники "ЕВРАЗ"
            </div>
            <div
              style="font-weight: bold"
              class="row q-gutter-xs"></div>

            <div
              style="font-weight: bold"
              class="row q-mb-md">
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

            <div
              style="font-weight: bold"
              class="row q-mb-md">
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

            <div
              style="font-weight: bold"
              class="row q-mb-md">
              <img
                style="width: 50px"
                src="https://avatars.mds.yandex.net/i?id=85e05f3c027cadf9e1d8a614850ed524a9a8bd66-9068341-images-thumbs&n=13"
                class="q-mr-sm"
              >
              База данных "ЕВРАЗ"
            </div>
          </q-card-section>
        </q-card>
      </div>

      <div class="col-8">
        <q-card
          class="text-white my-card"
          style="background: rgba(12, 37, 61, .95)"
        >
          <q-card-section>
            <apexchart type="line" height="480" :options="options3" :series="series3"/>
          </q-card-section>
        </q-card>
      </div>

      <div class="col-4">
        <div class="flex full-height" style="gap: 16px;">
          <div style="width: 48%;">
            <q-card
              class="my-card text-white full-height"
              style="background: rgba(12, 37, 61, .95)"
            >
              <q-card-section class="card">
                <div class="text-h5">ВХОДЯЩИЕ ЗВОНКИ</div>
                <div
                  style="color: limegreen"
                  class="textnumber">5
                </div>
                <div class="text-subtitle3">за неделю</div>
              </q-card-section>
            </q-card>
          </div>

          <div style="width: 48%;">
            <q-card
              class="my-card text-white full-height"
              style="background: rgba(12, 37, 61, .95)"
            >
              <q-card-section class="card">
                <div class="text-h5">ИСХОДЯЩИЕ ЗВОНКИ</div>
                <div
                  style="color: limegreen"
                  class="textnumber">5
                </div>
                <div class="text-subtitle4">за неделю</div>
              </q-card-section>
            </q-card>
          </div>

          <div style="width: 48%;">
            <q-card
              class="my-card text-white full-height"
              style="background: rgba(12, 37, 61, .95)"
            >
              <q-card-section class="card">
                <div class="text-h5">ПРИМЕЧАНИЙ</div>
                <div
                  style="color: limegreen"
                  class="textnumber">5
                </div>
                <div class="text-subtitle3">за неделю</div>
              </q-card-section>
            </q-card>
          </div>

          <div style="width: 48%;">
            <q-card
              class="my-card text-white full-height"
              style="background: rgba(12, 37, 61, .95)"
            >
              <q-card-section class="card">
                <div class="text-h5">УСПЕШНЫЕ СДЕЛКИ</div>
                <div
                  class="textnumber">3082
                </div>
                <div class="textnumber11" style="font-weight: bold">0 ₽</div>
                <div style="width: 50%;">
                  <hr>
                </div>
                <div class="textnumber2">+10</div>
                <div class="text-subtitle2">за неделю</div>
              </q-card-section>
            </q-card>
          </div>
        </div>
      </div>

      <div class="col-4">
        <q-card
          style="background: rgba(12, 37, 61, .95);"
          class="text-white my-card full-height"
        >
          <q-card-section>
            <div>
              <div class="text-h5">ИНДЕКС ПОТРЕБИТЕЛЬСКОЙ ЛОЯЛЬНОСТИ (NPS)</div>
            </div>
            <div style="width: 20%">
              <hr style="opacity: 5%">
            </div>

            <apexchart type="radialBar" height="350" :options="options4" :series="series4"></apexchart>
            <div>
              <div style="color: white">*NPS позволяет оценить уровень удовлетворенности клиентов Формула расчета: %
                Сторонников - % Критиков
              </div>
            </div>
          </q-card-section>
        </q-card>
      </div>

      <div class="col-4">
        <q-card
          class="text-white my-card full-height"
          style="background: rgba(12, 37, 61, .95)"
        >
          <q-card-section>
            <div>
              <div class="text-h5">ИСХОДЯЩИЕ СООБЩЕНИЯ ПО МЕНЕДЖЕРАМ</div>
              <div style="display:flex;justify-content: flex-end;color: limegreen"
                   class="textnumber">0
              </div>
              <div
                style="display:flex;justify-content: flex-end;"
                class="text-subtitle2">за неделю
              </div>
            </div>
            <div style="width: 20%">
              <hr>
            </div>
          </q-card-section>
        </q-card>
      </div>

      <div class="col-4">
        <q-card
          class="text-white my-card full-height"
          style="background: rgba(12, 37, 61, .95)"
        >
          <q-card-section>
            <div class="text-h5">ОБРАБОТАННЫЕ БЕСЕДЫ</div>
            <div style="display:flex;justify-content: flex-end;color: limegreen"
                 class="textnumber">0
            </div>
            <div
              style="display:flex;justify-content: flex-end;"
              class="text-subtitle2">за неделю
            </div>
            <div style="width: 20%">
              <hr>
            </div>
          </q-card-section>
        </q-card>
      </div>

      <div class="col-4">
        <q-card
          class="text-white my-card"
          style="background: rgba(12, 37, 61, .95); height: 400px;"
        >
          <q-card-section>
            <div>
              <div class="text-h5">ВХОДЯЩИЕ СООБЩЕНИЯ</div>
              <div style="width: 20%">
                <hr style="opacity: 5%; height: auto">
              </div>
            </div>
          </q-card-section>
        </q-card>
      </div>

      <div class="col-8">
        <q-card
          class="text-white my-card"
          style="background: rgba(12, 37, 61, .95); height: 400px;"
        >
          <q-card-section>
            <div>
              <div class="text-h5">СРЕДНЕЕ ВРЕМЯ ОТВЕТА</div>
              <div style="width: 20%">
              </div>
            </div>
          </q-card-section>
        </q-card>
      </div>
    </div>
  </div>
</template>


<script setup>
import {ref} from 'vue';

let options4 = {
  chart: {
    height: 200,
    type: 'radialBar',
  },
  plotOptions: {
    radialBar: {
      hollow: {
        size: '70%',
      },
      dataLabels: {
        show: true,
        name: {
          show: true,
          color: 'white',
        },
        value: {
          show: true,
          color: 'white'
        },
      },
    },
  },
  labels: ['NPS*'],

}

let series4 = [70]

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

let series5 = ref([25, 25, 25, 25])

let options5 = ref({
  chart: {
    height: 350,
    type: 'donut',
  },
  colors: ['#8B0000', '#FF8C00', '#FFFF99', 'lime '], // Цвета для каждой зоны
  plotOptions: {
    pie: {
      donut: {
        size: '65%', // Размер центрального отверстия
        labels: {
          show: false // Отключаем метки в центре
        }
      },
      startAngle: -90, // Начало дуги
      endAngle: 90,   // Конец дуги (полукруг),
      dataLabels: {
        offset: 40,
      }
    }
  },
  labels: ['25%', '50%', '75%', "100%"],
  dataLabels: {
    offsetY: 50,
    formatter: function (val, opts) {
      return opts.w.config.labels[opts.seriesIndex]
    },
    dropShadow: false,
    style: {
      fontSize: '12px',
      colors: ['#fff'],
      top: '50px'
    }
  },
  legend: {
    show: false // Отключаем легенду
  },
  // Кастомные метки для 25%, 50%, 75%, 100%
  annotations: {
    points: [
      {
        x: -135,
        y: 25,
        marker: {size: 0},
        label: {
          borderColor: '#777',
          offsetY: -20,
          offsetX: -30,
          style: {color: '#777', background: '#fff'},
          text: '25%'
        }
      },
      {
        x: -45,
        y: 50,
        marker: {size: 0},
        label: {
          borderColor: '#777',
          offsetY: -30,
          style: {color: '#777', background: '#fff'},
          text: '50%'
        }
      },
      {
        x: 45,
        y: 75,
        marker: {size: 0},
        label: {
          borderColor: '#777',
          offsetY: -30,
          style: {color: '#777', background: '#fff'},
          text: '75%'
        }
      },
      {
        x: 135,
        y: 100,
        marker: {size: 0},
        label: {
          borderColor: '#777',
          offsetY: -20,
          offsetX: 30,
          style: {color: '#777', background: '#fff'},
          text: '100%'
        }
      }
    ]
  },
  tooltip: {
    enabled: false // Отключаем всплывающие подсказки
  }
})

let series3 = ref([{
  name: "Desktops",
  data: [0, 15, 30,]
}])

let options3 = ref({
  chart: {
    toolbar: {
      show: false
    },
    background: 'transparent',
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
    text: 'ПРОГНОЗ ПРОДАЖ',
    align: 'left',
    style: {
      fontFamily: "PT Sans",
      color: 'white'
    },
  },
  grid: {
    row: {
      colors: ['transparent', 'transparent'], // takes an array which will be repeated on columns
    },
  },
  xaxis: {
    categories: ['сделок в работе сейчас', 'по прошествии 5 дней '],
    labels: {
      show: true,
      style: {
        fontFamily: "PT Sans",
        colors: ['white', 'white']
      },
      offsetX: 20,
    },

  },
  tooltip: {
    enabled: false,
  }
})
</script>

<style scoped>
.arrow {
  width: 50px;
  height: 100px;
  background-size: cover;
  background-repeat: no-repeat;
  background-image: url("./arrow.png");
  background-position: center;
  position: absolute;
  bottom: 175px;
  transform-origin: 50% 90%;
  //animation: rotate 7s ease-in-out infinite alternate;
}

.card {
  border-radius: 200px;
}

.container {
  margin: 40px auto;
  max-width: 1280px;
}

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
  opacity: 0.3;
  color: mediumpurple;

}

.text-number3 {
  opacity: 0.3;
  color: limegreen;
}

.text-number2 {
  opacity: 0.3;
  color: limegreen;
}

.text-number1 {
  opacity: 0.3;
  color: limegreen;
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

.my-card {
  border-radius: 10px;
}

.vdelo {
  margin-bottom: 30px;
  text-align: center;
  font-size: 40px;
  color: white;
  font-weight: bold;
}

.apexcharts-grid-row {
  fill: rgba(12, 37, 61, .95);
}
</style>
