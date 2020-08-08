<template>
  <div id="app">
    <Home />
  </div>
</template>

<script>
import Home from "./views/Home.vue";
export default {
  components: {
    Home,
  },
};
</script>

<style>
#app {
  width: 100%;
  height: 100%;
}

@font-face {
  font-family: "Muli";
  src: local("Muli"), url(./assets/fonts/Muli.ttf) format("truetype");
}
@font-face {
  font-family: "Muli-Light";
  src: local("Muli-Light"),
    url(./assets/fonts/Muli-Light.ttf) format("truetype");
}
@font-face {
  font-family: "Muli-Italic";
  src: local("Muli-Italic"),
    url(./assets/fonts/Muli-Italic.ttf) format("truetype");
}

body {
  font-family: Muli-Light;
}
</style>
