<template>
    <div class="col-6 col-lg-3">
        <h3>Important links</h3>
        <div class="red-line"></div>
        <p v-for="(element, index) in propLinks" :key="index">
          <a href="element.url">{{element.text}}</a>
        </p>
    </div>
</template>

<script>
export default {
    name: 'FooterLinks',
    props: {
      'propLinks' : Array
    }

}
</script>

<style lang="scss" scoped>
@import '../style/general.scss';
@import '../style/variables.scss';

h3{
  color: $total-white;
  font-size: 1.2rem;
}

p{
  color: $white-color-2-opac;
  font-weight: 300;
  font-size: 0.8rem;
  a{
    text-decoration: none;
    color: $white-color-2-opac;
  }
  a:hover{
    color: $red-color;
  }
}
.red-line{
  width: 30px;
  height: 1px;
  background-color: $red-color;
  margin: 15px 0;
}

</style>