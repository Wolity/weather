<script setup>
let city = defineModel()
</script>

<template>
  <nav>
    <div>
      <h2>PRECIPITATION</h2>
      <h3>0%</h3>
    </div>
    <div>
      <h2>HUMIDITY</h2>
      <h3>42%</h3>
    </div>
    <div>
      <h2>WIND</h2>
      <h3>3 km/h</h3>
    </div>
    <section>
      <main>
        <img src="../assets/Sun.png" />
        <h4>Tue</h4>
        <p>30 °C</p>
      </main>
      <main>
        <img src="../assets/Group.png" />
        <h4>Wed</h4>
        <p>22 °C</p>
      </main>
      <main>
        <img src="../assets/bi_cloud-rain.png" />
        <h4>Thu</h4>
        <p>06 °C</p>
      </main>
      <main>
        <img src="../assets/Sun.png" />
        <h4>Fy</h4>
        <p>26 °C</p>
      </main>
    </section>
    <label>
      <input v-model="city">
      <button @click="$emit('changeLocation',city.value)" class="btn">Change Location</button>
    </label>
  </nav>
</template>

<style lang="scss" scoped>
nav {
  background: #222831;
  width: 485px;
  height: 620px;
  border-radius: 0px 25px 25px 0px;
  padding: 60px 50px;
  div {
    margin-top: 15px;
    display: flex;
    justify-content: space-between;
  }
  h2 {
    color: white;
    font-size: 28px;
    font-weight: bold;
  }
  h3 {
    font-size: 24px;
    color: white;
  }
  section {
    padding-top: 85px;
    display: flex;
    width: 100%;
    justify-content: space-between;
    main{
      color: white;
      padding-top: 15px;
      padding-bottom: 30px;
      gap: 15px 0;
      border-radius: 10px;
      background: #272E37;
      align-items: center;
      width: 25%;
      display: flex;
      flex-direction: column;
    }
    p{
      font-weight: bold;
      font-size: 20px;
    }
    h4{
      font-size: 20px;
    }
  }
  label{
    margin-top: 75px;
    display: flex;
    flex-direction: column;
    .btn{
      filter: drop-shadow(0px 20px 15px #000000);
      border-radius: 10px;
      font-weight: bold;
      color: white;
      font-size: 20px;
      height: 55px;
      width: 400px;
      background: linear-gradient(45deg, #90D9E0, #5460E6);
    }
    input{
      filter: drop-shadow(0px 20px 15px #000000);
      border-radius: 10px;
      color: white;
      height: 30px;
      width: 400px;
      background: linear-gradient(45deg, #5460E6, #90D9E0);
    }
  }
}
</style>
