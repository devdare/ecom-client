<template>
  <div id="app" class="bg-blue-1050">
    <div id="nav">
      <Nav />
    </div>
    <div>
      <!-- <router-view></router-view> -->
    </div>
    <div>
      <Footer />
    </div>
  </div>
</template>

<script>
import Nav from "@/components/Nav";
import Footer from "@/components/Footer";
export default {
  components: { Nav, Footer },
};
</script>

<style lang="scss">
#app {
  font-family: "IBM Plex Sans", Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

html,
* {
  box-sizing: border-box;
}
body,
html {
  height: 100%;
  // width: 100vw;
  font-size: 62.5%;
  // max-width: 1200px;

  @media screen and (max-width: 1023px) {
    font-size: 56.25%;
  }
  @media screen and (max-width: 767px) {
    font-size: 50%;
  }
}

@media screen and (min-width: 1200px) {
  #App {
    margin-left: auto;
    margin-right: auto;
  }
}
</style>
