<template>
  <div id="app">
    <longScroll msg="So we did something a little earlier than expected?" style="padding-top: 300px"/>
    <longScroll msg="Is it a boy or a girl?"/>
    <longScroll msg="Keep scrolling to find out!"/>
    <h1>Ellie seemed to like what she saw</h1>
    <div style="padding-bottom: 1000px">
      <img src="~@/assets/ellie.png" height='403px' width='302px' style="border-radius: 25px" />
    </div>
    <clickReveal />
  </div>
</template>

<script>
import longScroll from './components/longScroll.vue'
import clickReveal from './components/clickReveal.vue'

export default {
  name: 'App',
  components: {
    longScroll,
    clickReveal,
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Abril+Fatface&display=swap');
html, body {
  height: 100%;
  margin: 0;
  margin-top: 0;
  padding: 0;
}

#app {
  font-family: "Abril Fatface", cursive, Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
