<template>
  <div class="home-container">
    <h1 class="welcome">Welcome to the best spot for corny Dad Jokes</h1>
    <nuxt-link class="call-to-action" to="/jokes"
      >Click here to see jokes</nuxt-link
    >
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: "Home"
    };
  }
};
</script>

<style>
body {
  background-image: url(".././assets/imgs/backg3.jpg");
  background-position: center;
  background-size: cover;
  background-attachment: fixed;
  background-repeat: no-repeat;
  color: white;
}
.welcome {
  margin-top: 30px;
  font-size: 50px;
  width: fit-content;
  text-shadow: -2px -2px black;
}
.call-to-action {
  color: white;
  background: #183585;
  text-decoration: none;
  padding: 10px;
  border-radius: 5px;
  font-size: 20px;
  width: fit-content;
  border: 2px solid white;
  margin-top: 5%;
  transition: 0.3s;
}

.call-to-action:hover {
  color: white;
  background: green;
}

.home-container {
  display: flex;
  justify-content: center;
  flex-direction: column;
  padding-top: 10%;
  align-items: center;
}
</style>
