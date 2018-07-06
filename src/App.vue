<template>
  <div id="app">
    <Header />
    <NavBar src="hit" />
    <Hero headline="Hi, From Props" details="This is interesting" cta="Contact Us" /> 
    <MainTent></MainTent>
     <lazyImage src="https://imgplaceholder.com/425x250/ff7f7f/333333/fa-image" className="mega-image" alt="lazyload">
    </lazyImage> 
    	<s-video controls="controls" width="100%" poster="https://source.unsplash.com/user/erondu/200x200" src="http://techslides.com/demos/sample-videos/small.mp4">
      </s-video>
      <Footer></Footer>
  </div>
</template>

<script>
import Header from "./components/header";
import NavBar from "./components/navbar";
import Hero from "./components/hero";
import MainTent from "./components/main-content";
import lazyImage from "./components/lazy-images";
import sVideo from "./components/s-video";
import Footer from "./components/footer";

export default {
  name: "App",
  components: {
    Header,
    NavBar,
    Hero,
    lazyImage,
    sVideo,
    Footer,
    MainTent
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  max-width:1180px;
  margin:0 auto;
}
</style>
