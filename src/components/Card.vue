<script setup></script>

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
        <img src="" />
        <h4>Tue</h4>
        <p>30 °C</p>
      </main>
      <main>
        <img src="" />
        <h4>Wed</h4>
        <p>22 °C</p>
      </main>
      <main>
        <img src="" />
        <h4>Thu</h4>
        <p>06 °C</p>
      </main>
      <main>
        <img src="" />
        <h4>Fy</h4>
        <p>26 °C</p>
      </main>
    </section>
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
}
</style>
