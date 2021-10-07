<template>
    <div class="col-6 col-lg-3 mb-3">
        <h3>Twitter</h3>
        <div class="red-line"></div>
        <div class="d-flex justify-content-between">
            <i class="fab fa-twitter"></i>
            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Iusto libero ea incidunt corporis illo nostrum eligendi molestiae magnam iure at.</p>
        </div>
        <div class="d-flex justify-content-between">
            <i class="fab fa-twitter"></i>
            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Iusto libero ea incidunt corporis illo nostrum eligendi molestiae magnam iure at.</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FooterTwitter'

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
  margin-bottom: 30px;
}
.red-line{
  width: 30px;
  height: 1px;
  background-color: $red-color;
  margin: 15px 0;
}

i{
    padding-right: 30px;
    color: $red-color;
}

</style>