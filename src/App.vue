<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <CounterPage />
</template>

<script>
import { defineAsyncComponent } from "vue";

export default {
  name: "App",
  components: {
    CounterPage: defineAsyncComponent(() =>
      import("@/components/CounterPage.vue")
    ),
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
