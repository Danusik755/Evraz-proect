<template>
  <q-page class="flex flex-center">
    <button>Сделать по приколу</button>
    <input placeholder="Написать по приколу">
    <div class="gaga">
      <button>Добавить по приколу</button>
    </div>
    <apexchart type="bar" height="350" :options="{ xaxis: { categories: ['test1', 'test2']}}" :series="[{ name: 'test', data: [ 30, 40]}]"/>
  </q-page>

</template>

<script setup>

</script>
