<template>
  <div id="app">
    <Panel />
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>

    <router-view />
  </div>
</template>

<script>
// @ is an alias to /src
import Panel from "@/components/panel.vue";

export default {
  components: {
    Panel,
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
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}

#square {
  width: 100px;
  height: 100px;
  background: Url("https://www.infpol.ru/upload/iblock/313/3132a7b76ec702b6b81fc34d5bc8bf9e.jpg");
  background-size: cover;
  border-radius: 50%;
}
</style>
