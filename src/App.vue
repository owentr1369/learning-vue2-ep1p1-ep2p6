<template>
  <div id="app">
    <h1>Hello</h1>
    <div id="obj">
      <p v-html="something.textMaHTML"></p>
      <p v-once>{{ something.noidung }} - {{ showPost() }}</p>
      <a v-bind:href="something.link">Hello</a>
    </div>
  </div>
</template>

<script>
export default {
  // Tat ca du lieu truyen qua html deu o da du lieu tho
  name: "App",
  data() {
    return {
      something: {
        noidung: "Chao cac ban",
        title: "Blablablabla",
        link: "https://facebook.com",
        textMaHTML: '<a href="https....awdasd">Get password</a>',
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
