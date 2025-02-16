<script setup>
import Waves from "./components/Waves.vue"
import Card from "./components/Card.vue"
</script>

<template>
  <link
    rel="stylesheet"
    href="https://pro.fontawesome.com/releases/v5.15.2/css/all.css"
/>
  <main>
  <Waves/>
  <Card/>
  <i class="far fa-sun"></i>
  </main>
</template>

<style lang="scss">
body {
  background: #343d4b;
  display: flex;
  justify-content:center;
  align-items: center;
  height: 100vh;
}
main{
  align-items: center;
  display: flex;
}
</style>
