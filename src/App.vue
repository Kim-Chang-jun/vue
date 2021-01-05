<template>
  <div id="app">
    <HelloWorld
      msg="어뮤즈트래블은 돌봄여행을 제공하는 컨시어지 여행사입니다"
    />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
  },
};
</script>

<style>
#app {
  height: 100vh;
  display: flex;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background-color: brown;
}
</style>
