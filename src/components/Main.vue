<template>
    <main>
      <div class="base-page">
        <OurSpecialties :propSpecialties="specialties" />
      </div>
    </main>
</template>

<script>
import OurSpecialties from './OurSpecialties.vue';

export default {
  name: "Main",
  components: {
    OurSpecialties
  },
  data() {
    return {
      specialties: [
        {
          icon: '../assets/svg/svg-0.svg',
          title: 'Knowing',
          text: 'Lorem ipsum dolor sit amet, quis consect.'
        },
        {
          icon: '../assets/svg/svg-0.svg',
          title: 'Knowing',
          text: 'Lorem ipsum dolor sit amet, quis consect.'
        },
        {
          icon: '../assets/svg/svg-0.svg',
          title: 'Knowing',
          text: 'Lorem ipsum dolor sit amet, quis consect.'
        },
        {
          icon: '../assets/svg/svg-0.svg',
          title: 'Knowing',
          text: 'Lorem ipsum dolor sit amet, quis consect.'
        }
      ]
    }
  }

};
</script>


<style scoped lang="scss">
@import '../style/general.scss';
@import '../style/variables.scss';

.base-page{
  height: 100vh;
  background-color: $white-color-6;
  position: relative;
}


</style>