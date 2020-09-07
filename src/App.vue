<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="test" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld
  },
  el: '#list1',
  data: function (){
    return{
    items: [
      { list: 'ulタグ及びolタグは、liタグを含めることでリスト表現できる。'},
      { list: 'ulタグはUnorderList、即ち順序・順番に無関係のリストを作成'},
      { list: 'olタグはOderList、即ち順序・順番に関係あるリストを作成'},
      { list: 'ul、ol、liには注意がある'}
    ]}
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
