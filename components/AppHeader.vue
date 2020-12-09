<template lang="">
  <header>
    <h1 class="title">Dad Jokes</h1>
    <div class="menu">
      <nuxt-link to="/">Home</nuxt-link>
      <nuxt-link to="/jokes">Jokes</nuxt-link>
      <nuxt-link to="/about">About</nuxt-link>
    </div>
  </header>
</template>
<script>
export default {
  name: "AppHeader"
};
</script>
<style>
header {
  display: flex;
  justify-content: space-between;
  border-bottom: 1px solid grey;
  background-color: #ebebeb;
  padding: 0;
  margin: 0;
  padding-left: 30px;
  padding-right: 30px;
}
.menu {
  display: flex;
  align-items: center;
}
a {
  text-decoration: none;
  color: grey;
  border: 1px solid grey;
  border-radius: 5px;
  padding: 10px;
  margin: 10px;
  transition: 0.3s;
  background: white;
}
a:hover {
  color: #e87f22;
  border: 1px solid #e87f22;
}
.title {
  color: #3774be;
}
</style>
