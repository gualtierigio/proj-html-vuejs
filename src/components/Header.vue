<template>
    <header id="jumbotron-header">
      <Navbar :propNavMenu ='navMenu'/>
      <HeaderContent />
      <div class="white-bar"></div>
    </header>
</template>

<script>
import Navbar from './Navbar.vue';
import HeaderContent from './HeaderContent.vue';

export default {
  name: "Header",
  components: {
    Navbar,
    HeaderContent
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
  background-size: cover;
  background-position: center;
}

.white-bar{
  width: 90%;
  margin: 0 auto;
  background-color: $total-white;
  height: 100px;
  z-index: 10;
}

</style>
