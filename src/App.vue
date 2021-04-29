<template>
  <div class="container">
    <HelloWorld msg="hello" />
    <hr>
    <TwitterEmbed />
    <hr>
    <div class="controls">
      <ScreenShot /> <SendScreen />
    </div>
    <hr>
    <Details />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import TwitterEmbed from "./components/TwitterEmbed.vue";
import ScreenShot from "./components/ScreenShot.vue";
import Details from "./components/Details.vue";
import SendScreen from "./components/SendScreen.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    TwitterEmbed,
    ScreenShot,
    Details,
    SendScreen
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0;
}
.controls div {
  display: inline-block;
}
</style>
