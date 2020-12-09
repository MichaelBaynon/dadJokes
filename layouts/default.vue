<template>
  <div>
    <AppHeader />
    <Nuxt />
  </div>
</template>

<script>
import AppHeader from "../components/AppHeader";

export default {
  components: {
    AppHeader
  }
};
</script>

<style>
body {
  padding: 0;
  margin: 0;
  font-family: sans-serif;
}
</style>
