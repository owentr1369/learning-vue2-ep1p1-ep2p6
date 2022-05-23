<template>
  <div id="app">
    <h1>Hello</h1>
    <div id="obj">
      <p>{{ something.title }}</p>
      <p v-once>{{ something.noidung }} - {{ showPost() }}</p>
      <a v-bind:href="something.link">Hello</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      something: {
        noidung: "Chao cac ban",
        title: "Blablablabla",
        link: "https://facebook.com",
      },
    };
  },
  methods: {
    showPost: function () {
      this.noidung = "Noi dung moi duoc cap nhat";
      return this.noidung;
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
