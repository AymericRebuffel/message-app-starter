<template>
  <div class="app">
    <Messages/>
    <Menu/>
  </div>
</template>

<script>

import Messages from "@/components/Messages";
import Menu from "@/components/Menu";

export default {
  name: "App",
  components: {
    Menu,
    Messages
  }
};
</script>

<style>
html, body {
  height: 100%;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
