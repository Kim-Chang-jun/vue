<template>
  <div class="hello">
    <h1>{{ text }}</h1>
    <div id="example-1">
      <button v-on:click="click">Add 1</button>
    </div>
  </div>
</template>


<script>

export default {
  name: "HelloWorld",
  props: {
    msg: String,
    msg2: String,
  },
  data() {
    return {
      text: "어뮤즈트래블은 돌봄여행을 제공하는 컨시어지 여행사입니다",
    };
  },
  methods: {
    click: function () {
      var textArray = this.text.split("");
      var popText = textArray.shift();
      textArray.push(popText);
      console.log(textArray);
      this.text = textArray.join("");
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello {
  width: 100%;
  text-align: center;
  align-self: center;
  justify-self: center;
}
</style>
