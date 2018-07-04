<template>
  <div id="app">
    <Header />
    <NavBar src="hit" />
    <Hero headline="Hi, From Props" details="This is interesting" cta="Contact Us" /> 
    <MainTent></MainTent> 
  </div>
</template>

<script>
import Header from "./components/header";
import NavBar from "./components/navbar";
import Hero from "./components/hero";
import MainTent from "./components/main-content";

export default {
  name: "App",
  components: {
    Header,
    NavBar,
    Hero,
    MainTent
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
