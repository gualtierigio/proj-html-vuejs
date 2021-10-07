<template>
    <footer>
      <div class="page-wrap">
        <div class="container">
          <div class="row gx-5">
            <div class="col-6 col-lg-3">
              <h3>About</h3>
              <div class="red-line"></div>
              <p>We created Everlead to effectly become the stepping stone towards meeting all your goals & achieving business succes.</p>
              <div class="socials"></div>
            </div>
            <div class="col-6 col-lg-3">
              <h3>Twitter</h3>
              <div class="red-line"></div>
            </div>
            <div class="col-6 col-lg-3">
              <h3>Important links</h3>
              <div class="red-line"></div>
            </div>
            <div class="col-6 col-lg-3">
              <h3>Contact me</h3>
              <div class="red-line"></div>
            </div>
          </div>
        </div>
      </div>
    </footer>
</template>

<script>
export default {
  name: "Footer",

};
</script>


<style scoped lang="scss">
@import '../style/general.scss';
@import '../style/variables.scss';

footer{
  background-color: $black-color-2;
  height: 50vh;
  width: 100%;
  padding-top: 100px;
}

.page-wrap{
  border: 1px solid red;
  width: 65%;
  margin: 0 auto;
}

h3{
  color: $total-white;
  font-size: 1.2rem;
}

p{
  color: $white-color-2-opac;
  font-weight: 300;
  font-size: 0.8rem;
}
.red-line{
  width: 30px;
  height: 1px;
  background-color: $red-color;
  margin: 15px 0;
}

</style>