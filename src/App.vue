<script setup>
import Waves from "./components/Waves.vue"
import Card from "./components/Card.vue"
</script>

<template>
  <main>
  <Waves/>
  <Card/>
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
