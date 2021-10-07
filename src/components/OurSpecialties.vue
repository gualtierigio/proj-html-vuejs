<template>
  <div id="ourSpecialties_container">
      <div class="specialties_intro">
          <h1>Our Specialtiesspan<span class="red-dot">.</span></h1>
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ipsum debitis perferendis vitae.</p>
      </div>

  </div>
</template>

<script>
export default {
    name: 'OurSpecialties',
}
</script>

<style scoped lang="scss">
@import '../style/general.scss';
@import '../style/variables.scss';

#ourSpecialties_container{
    width: 90%;
    margin: 0 auto;
    background-color: $total-white;
    padding: 150px 0;
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



.red-dot{
  color: $red-color;
}

</style>