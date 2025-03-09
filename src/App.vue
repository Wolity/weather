<script setup>
import Waves from "./components/Waves.vue";
import Card from "./components/Card.vue";
import { ref } from "vue";
let info = ref()
async function weather() {
  let request = await fetch(
    "https://api.openweathermap.org/data/2.5/forecast?q=Kaliningrad&cnt=40&appid=1e9a174f92c5f2ce16b22391ff3531c8&units=metric"
  );
   info.value = await request.json()
  console.log(info)
}
weather()
</script>

<template>
  <link
    rel="stylesheet"
    href="https://pro.fontawesome.com/releases/v5.15.2/css/all.css"
  />
  <main>
    <Waves :info = "info" />
    <Card />
  </main>
</template>

<style lang="scss">
body {
  background: #343d4b;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}
main {
  align-items: center;
  display: flex;
}
</style>
