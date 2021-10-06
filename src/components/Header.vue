<template>
    <header id="jumbotron-header">
      <Navbar />
      <HeaderContent />
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
