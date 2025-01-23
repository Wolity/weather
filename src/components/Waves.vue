<script setup></script>

<template>
  <nav class="waves">
    <img class = "waves_img" src="../assets/waves.png" />
    <div class="waves_info">
      <h1>Tuesday</h1>
      <span>20 Jun 2025</span>
      <h2>Biarritz, FR</h2>
    </div>
    <div class="waves_weather">
      <img src="../assets/sun.png" />
      <h2>29 °C</h2>
      <h3>Sunny</h3>
    </div>
  </nav>
</template>

<style lang="scss">
.waves {
    .waves_img{

    }
    position: relative;
  .waves_info {
    top: 0;
    position: absolute;
  }
  .waves_weather {
    bottom: 0;
    position: absolute;
  }
}
</style>
