<template>
    <header id="jumbotron-header">
      <Navbar />
    </header>
</template>

<script>
import Navbar from './Navbar.vue';

export default {
  name: "Header",
  components: {
    Navbar
  },
  data() {
    return {
      navMenu: [
        {
          text: "home",
          url: "#home",
        },
        {
          text: "pages",
          url: "#pages",
        },
        {
          text: "blog",
          url: "#blog",
        },
        {
          text: "shop",
          url: "#shop",
        },
        {
          text: "events",
          url: "#events",
        },
        {
          text: "elements",
          url: "#elements",
        }
      ]
    }
  }

};
</script>


<style scoped lang="scss">
@import '../style/general.scss';
@import '../style/variables.scss';

#jumbotron-header{
  background-image: url(../assets/img/rev-slider-main-home-img-03.jpg);
  width: 100%;
  height: 95vh;
  background-size: cover;
  background-position: center;
}

</style>
