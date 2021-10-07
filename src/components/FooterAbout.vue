<template>
  <div class="col-6 col-lg-3 mb-3">
    <h3>About</h3>
    <div class="red-line"></div>
    <p>We created Everlead to effectly become the stepping stone towards meeting all your goals & achieving business succes.</p>
        <div class="socials d-flex">
            <div class="social-custom">
                <i class="fab fa-twitter"></i>
            </div>
            <div class="social-custom">
                <i class="fab fa-facebook-f"></i>
            </div>
            <div class="social-custom">
                <i class="fab fa-linkedin-in"></i>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FooterAbout'

}
</script>

<style lang="scss" scoped>
@import '../style/general.scss';
@import '../style/variables.scss';

.social-custom{
  width: 25px;
  height: 25px;
  background-color: $total-white;
  border-radius: 50%;
  margin-right: 10px;
  position: relative;
  i{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
  }
}

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

</style>