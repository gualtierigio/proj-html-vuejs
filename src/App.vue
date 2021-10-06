<template>
  <div id="app">
    <Headerd />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Headerd from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Headerd,
    Main,
    Footer
  },
};
</script>

<style lang="scss">
@import './style/general.scss';
@import './style/variables.scss';

#app{
  font-family: $font-page;
}


</style>
