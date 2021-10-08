<template>
  <div id="ourSpecialties_container">
      <div class="specialties_intro">
          <h1>Our Specialties<span class="red-dot">.</span></h1>
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ipsum debitis perferendis vitae.</p>
          <div class="red-line"></div>
      </div>
      <div class="specialties_props-wrapper">
          <div class="container">
              <div class="row gx-5">
                  <!-- <div v-for="(element, index) in propSpecialties" :key="index" class="col-6 col-lg-3 specialties__content">
                      <img :src="element.icon" alt="icon specialties">
                      <h3>{{element.title}}</h3>
                      <p>{{element.text}}</p>
                  </div> -->
                  <div class="col-6 col-lg-3 specialties__content">
                      <img src="../assets/svg/svg-0.svg" alt="icon specialties">
                      <h3>Knowing</h3>
                      <p>Lorem ipsum dolor sit amet, quis consect.</p>
                  </div>
                  <div class="col-6 col-lg-3 specialties__content">
                      <img src="../assets/svg/svg-1.svg" alt="icon specialties">
                      <h3>Selling</h3>
                      <p>Lorem ipsum dolor sit amet, quis consect.</p>
                  </div>
                  <div class="col-6 col-lg-3 specialties__content">
                      <img src="../assets/svg/svg-2.svg" alt="icon specialties">
                      <h3>Learning</h3>
                      <p>Lorem ipsum dolor sit amet, quis consect.</p>
                  </div>
                  <div class="col-6 col-lg-3 specialties__content">
                      <img src="../assets/svg/svg-3.svg" alt="icon specialties">
                      <h3>Contact</h3>
                      <p>Lorem ipsum dolor sit amet, quis consect.</p>
                  </div>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'OurSpecialties',
    props: {
        'propSpecialties' : Array
    }
}
</script>

<style scoped lang="scss">
@import '../style/general.scss';
@import '../style/variables.scss';

#ourSpecialties_container{
    width: 90%;
    margin: 0 auto;
    background-color: $total-white;
    padding: 50px 100px 150px 100px;
    min-width: 620px;
}

.specialties_intro{
    text-align: center;
    h1{
        font-size: 3.2rem;
        font-weight: bold;
        margin-bottom: 30px;
    }
    p{
        font-size: 0.9rem;
        font-weight: 300;
        color: $gray-text-color-1;
    }
}

.specialties_props-wrapper{
    margin-top: 100px;
}

.specialties__content{
    text-align: center;
    h3{
       font-size: 1rem;
       font-weight: bold;
       margin-bottom: 20px;
    }
    p{
        font-size: 0.9rem;
        font-weight: 300;
        color: $gray-text-color-1;
    }
    img{
        margin-bottom: 50px;
    }
}

// specific implementation

.red-line{
  width: 100px;
  height: 2px;
  background-color: $red-color;
  margin: 0 auto;
}

.red-dot{
  color: $red-color;
}

</style>