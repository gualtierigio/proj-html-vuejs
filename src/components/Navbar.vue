<template>
    <div class="d-flex" id="top-header">
        <a href="#"><h1>Everlead<span class="red-dot">.</span></h1></a>
        <nav>
          <ul>
            <li id="collaps-menu" v-for="(element, index) in propNavMenu" :key="index">
              <a href="{link.url}">
                <div>
                  <i class="fas fa-long-arrow-alt-right"></i>
                </div>{{element.text}}
              </a>
            </li>
            <li class="fas-elements">
              <a href="#"><i class="fas fa-search"></i></a>
            </li>
            <li class="fas-elements">
              <a href="#"><i class="fas fa-bars"></i></a>
            </li>
          </ul>
        </nav>
    </div>
</template>

<script>
export default {
  name: "Navbar",
  props: {
    'propNavMenu' : Array
  }
};
</script>


<style scoped lang="scss">
@import '../style/general.scss';
@import '../style/variables.scss';

#top-header{
  width: 100%;
  height: 100px;
  align-items: center;
  justify-content: space-between;
  padding: 0 50px;
}

h1{
    font-size: 1.7rem;
    font-weight: bold;
}

nav{
  text-transform: uppercase;
  font-size: 0.8rem;
  font-weight: bold;

  ul{
    li{
      display: inline-block;
      padding-left: 10px;
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

// logo red

a:hover{
    color: $red-color;
}

.fas-elements{
    padding-left: 30px;
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
