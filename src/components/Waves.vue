<script setup>
defineProps({
  info: Object,
});
</script>

<template>
  <nav class="waves">
    <img class="waves_img" src="../assets/waves.png" />
    <div class="waves_info">
      <h1>Tuesday</h1>
      <span>20 Jun 2025</span>
      <h2>{{ info.city.name }},   {{ info.city.country }}</h2>
    </div>
    <div class="waves_weather">
      <img class="wave_picture" src="../assets/sun.png" />
      <h2>{{ info.list[0].main.temp }} °C</h2>
      <h3>{{ info.list[0].weather[0].main }}</h3>
    </div>
  </nav>
  <!-- {{ info.city.country }} -->
</template>

<style lang="scss" scoped>
.waves {
  .waves_img {
  }
  position: relative;
  .waves_info {
    padding-top: 45px;
    padding-left: 30px;
    top: 0;
    position: absolute;
    h1 {
      padding-bottom: 15px;
      color: white;
      font-size: 37px;
      font-weight: bold;
    }
    span {
      font-size: 20px;
      color: white;
    }
    h2 {
      padding-top: 15px;
      font-size: 22px;
      color: white;
    }
  }
  .waves_weather {
    padding-left: 30px;
    padding-bottom: 85px;
    bottom: 0;
    position: absolute;
    .wave_picture {
      width: 95px;
    }
    h2 {
      padding-top: 10px;
      color: white;
      font-weight: bold;
      font-size: 50px;
    }
    h3 {
      padding-top: 15px;
      color: white;
      font-weight: bold;
      font-size: 30px;
    }
  }
}
</style>
