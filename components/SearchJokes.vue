<template>
  <div>
    <form class="search-form" @submit.prevent="onSubmit">
      <input
        class="search-box"
        type="text"
        v-model="text"
        placeholder="search"
      />
      <input class="submit-button" type="submit" value=" 🔍 Search Jokes" />
    </form>
  </div>
</template>
<script>
export default {
  name: "SearchJokes",
  data() {
    return {
      text: ""
    };
  },
  methods: {
    onSubmit() {
      this.$emit("search-text", this.text);
      this.text = "";
    }
  }
};
</script>
<style>
.search-box {
  padding: 12px;
  background: #ebebeb;
  border: 1px solid grey;

  border-radius: 5px;
  font-size: 20px;
  margin-right: 30px;
}

.search-form {
  display: flex;
  margin: 0 auto;
  margin-top: 30px;
  margin-bottom: 30px;

  width: fit-content;
}

.submit-button {
  border-radius: 50px;
  border: none;
  background: #1f2263;
  border: 2px solid white;
  color: white;
  font-size: 15px;
  padding-left: 10px;
  padding-right: 20px;
  transition: 0.3s;
}
.submit-button:hover {
  background: crimson;
  cursor: pointer;
}
</style>
