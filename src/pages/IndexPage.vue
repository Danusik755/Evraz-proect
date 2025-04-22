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
      <div class="text-h6">ВЫПОЛНЕННЫЕ ЗАДАЧИ</div>
      <div class="textnumber">0</div>
      <div class="text-subtitle2">за неделю</div>
    </q-card-section>
      </q-card>
    </div>
  </div>





</template>
<!--  <q-page class="flex flex-center">-->
<!--    <apexchart type="bar" height="350" width='500' :options="options" :series="series"/>-->
<!--    <apexchart type="donut"  width='500' :options="options2" :series="series2"/>-->
<!--  </q-page>-->



<script setup>

import { ref } from 'vue';




// let series = ref([
//   {
//     name: 'test',
//     data: [ 30, 40,50,43,65,84,14,98,35]
//   }
//   ]
// )
//
// let options= ref({ xaxis: { categories: ['test1', 'test2', 'test3','test4','test5','test6','test7','test8','test9',]}})
//
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

.card {
}
</style>
