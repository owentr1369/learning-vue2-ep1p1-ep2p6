<template>
  <div id="app">
    <h1>Hello</h1>
    <div id="obj">
      <p>{{ showPost() }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      noidung: "Chao cac ban",
      title: "Blablablabla",
    };
  },
  methods: {
    showPost: function () {
      return this.title;
    },
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
