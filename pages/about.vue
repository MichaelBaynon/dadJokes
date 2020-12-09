<template>
  <div class="about">
    Site was made and maintained by
    <a href="https://github.com/MichaelBaynon" target="_">Michael Baynon</a>
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: "About"
    };
  }
};
</script>

<style>
.about {
  font-size: 25px;
  margin: 0 auto;
  width: fit-content;
  margin-top: 22%;
  text-shadow: -1px -1px black;
}
a {
  color: #6c41bf;
}
.about a:hover {
  color: purple;
}
</style>
