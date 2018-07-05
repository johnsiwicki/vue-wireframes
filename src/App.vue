<template>
  <div id="app">
    <Header />
    <NavBar src="hit" />
    <Hero headline="Hi, From Props" details="This is interesting" cta="Contact Us" /> 
    <MainTent></MainTent>
    <lazyImage src="http://via.placeholder.com/450x150" className="mega-image" alt="lazyload">
    </lazyImage> 

    	<s-video controls="controls" width="100%" poster="https://source.unsplash.com/user/erondu/400x400" src=""></s-video>
  </div>
</template>

<script>
import Header from "./components/header";
import NavBar from "./components/navbar";
import Hero from "./components/hero";
import MainTent from "./components/main-content";
import lazyImage from "./components/lazy-images";
import sVideo from "./components/s-video";


export default {
  name: "App",
  components: {
    Header,
    NavBar,
    Hero,
    lazyImage,
    sVideo,
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
