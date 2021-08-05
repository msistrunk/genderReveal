<template>
  <div class="scroll">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
export default {
  name: 'longScroll',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.scroll {
    padding-bottom: 1500px
}
</style>
