<template>
  <div class="scroll">
    <h1>{{ message }}</h1>
    <button class="button" v-if="showButton" v-on:click="count++">click</button>
    <img v-else src="~@/assets/ultrasound.jpg" height='283px' width='373px' style="border-radius: 25px" />
  </div>
</template>

<script>
export default {
  name: "clickReveal",
  data: function () {
    return {
      message: "Click the button to reveal!",
      count: 0,
      showButton: true,
    };
  },
  watch: {
    
    count: function (val) {
      if (val == 0) {
        this.message = "Click the button to reveal!";
      } else if (val == 1) {
        this.message = "keep clicking!!!";
      } else if (val > 30) {
        this.message = "IT'S A BOY!";
        this.showButton = false;
      } else if (val > 25) {
        this.message = "here it is!";
      } else if (val > 20) {
        this.message = "ok really almost there!";
      } else if (val > 15) {
        this.message = "getting tired yet?";
      } else if (val > 10) {
        this.message = "getting closer!";
      } else if (val > 5) {
        this.message = "almost there!!!";
      } else if (val > 3) {
        this.message = "keep going!!!";
      }
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.scroll {
  padding-bottom: 1500px;
}
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

.button {
  background-color: #2c3e50;
  font-family: "Abril Fatface", cursive, Avenir, Helvetica, Arial, sans-serif;
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 30px;
  margin: 4px 2px;
  cursor: pointer;
  border-radius: 10px;
}
</style>
