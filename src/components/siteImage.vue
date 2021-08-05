<template>
  <div class="scroll">
    <h1>{{ msg }}</h1>
    <img :src=src :height=height :width=width>
  </div>
</template>

<script>
export default {
  name: 'siteImage',
  props: {
    msg: String,
    src: String,
    height: String,
    width: String,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.scroll {
    padding-bottom: 1500px
}
</style>
