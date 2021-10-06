<template>
    <header id="jumbotron-header">
      <div class="d-flex" id="top-header">
        <a href="#"><h1>Everlead<span class="red-dot">.</span></h1></a>
        <nav>
          <ul>
            <li id="collaps-menu" v-for="(element, index) in navMenu" :key="index">
              <a href="{link.url}">
                <div id="arrow">
                  <i class="fas fa-long-arrow-alt-right"></i>
                </div>{{element.text}}
              </a>
            </li>
            <li>
              <a href="#"><i class="fas fa-search"></i></a>
            </li>
            <li>
              <a href="#"><i class="fas fa-bars"></i></a>
            </li>
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

#top-header{
  width: 100%;
  height: 160px;
  align-items: center;
  justify-content: space-between;
  padding: 0 30px;
}

nav{
  text-transform: uppercase;
  ul{
    li{
      display: inline-block;
      padding: 0 20px;
      a{
        div{
        width: 20px;
        display: inline-block;
        i{
          display: none;
        }
      }
      }
      a:hover{
        color: $red-color;
        div i{
          display: block;
        }
      }
    }
  }
}

a:hover{
  color: $red-color;
}

@media screen and (max-width: 1150px) {
  #collaps-menu{
    display: none;
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
