<template>
    <header id="jumbotron-header">
      <div class="d-flex" id="top-header">
        <a href="#"><h1>Everlead<span class="red-dot">.</span></h1></a>
        <nav>
          <ul>
            <li v-for="(element, index) in navMenu" :key="index">{{element.index}}</li>
          </ul>
        </nav>
      </div>
    </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      navMenu: [
        'home',
        'pages',
        'blog',
        'shop',
        'events',
        'elements'
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

#top-header{
  width: 100%;
  height: 200px;
  align-items: center;
  justify-content: space-between;
  border: 1px solid red;
}

nav{
  ul{
    li{
      display: inline-block;
      width: 30px;
      border: 1px solid red;
      padding: 0 20px;
    }
  }
}

a{
  text-decoration: none;
  color: $total-black;
}

.red-dot{
  color: $red-color;
}

</style>
