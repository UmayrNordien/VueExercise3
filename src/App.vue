<template>
  <NavBarVue></NavBarVue>
  <router-view/>
  <FooterVue></FooterVue>
</template>

<script>
import NavBarVue from './components/NavBar.vue';
import FooterVue from './components/Footer.vue';

export default{
  components: {
    NavBarVue,
    FooterVue,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #1c1a1a;
}

body{
  background-color: #9e9e9e;
}

nav {
  padding: 10px;
}

nav a {
  font-weight: bold;
  color: #1c1a1a;
}

nav a.router-link-exact-active {
  color: #ffffff;
}
</style>
