<template>
  <nav>
    <NavBarVue></NavBarVue>
    <router-view />
    <FooterVue></FooterVue>
  </nav>
</template>


<script>
import NavBarVue from '@/components/NavBar.vue';
import FooterVue from '@/components/Footer.vue';

export default {
  components: {
    NavBarVue,
    FooterVue,
}
}
</script>


<style>
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  font-family: 'Caveat', cursive;
    font-family: 'Pathway Gothic One', sans-serif;
    font-family: 'Sedgwick Ave Display', cursive;
}

body{
  background: rgb(253,255,135);
  background: linear-gradient(90deg, rgba(253,255,135,1) 27%, rgba(255,151,212,1) 56%, rgba(131,255,218,1) 94%);
}

nav {
  padding: 0px;
  margin:0;
}

nav a {
  font-weight: bold;
  color: #000000;
}

nav a.router-link-exact-active {
  color:  rgba(255,131,227,1);
}

a:hover {
  color: rgba(131,255,218,1);
}
</style>
