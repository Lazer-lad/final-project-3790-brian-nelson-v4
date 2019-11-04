<template>
  <v-app>
    <v-app-bar app color="secondary" dark>
      <div id="app">{{ info }}</div>
    </v-app-bar>

    <v-content></v-content>
    <About></About>
  </v-app>
</template>

<script>
//import HelloWorld from './components/HelloWorld';
import About from "./views/About";

export default {
  name: "App",

  components: {
    //HelloWorld,
    About,
  },

  data: () => ({
    //
  })
};
</script>
