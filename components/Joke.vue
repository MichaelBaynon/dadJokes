<template>
  <nuxt-link class="joke-link" :to="'jokes/' + id">
    <div class="joke">
      <p>{{ joke }}</p>
      <span class="tooltiptext">Click for more information</span>
    </div>
  </nuxt-link>
</template>
<script>
export default {
  name: "Joke",
  props: ["joke", "id"]
};
</script>
<style>
.joke {
  padding: 0.1rem;
  border-radius: 5px;
  border: 1px solid lightgrey;
  margin: 1rem 0;
  display: flex;
  color: black;
  transition: 0.3s;
  align-items: center;
  background: #ebebeb;
  width: 45%;
  margin: 1rem auto;
}

.tooltiptext {
  color: green;
  margin-left: 50px;
  font-size: 20px;
  visibility: hidden;
}
.joke:hover .tooltiptext {
  visibility: visible;
}

.joke p {
  margin-left: 50px;
  width: fit-content;
}

.joke-link {
  text-decoration: none;
  width: fit-content;
}
</style>
