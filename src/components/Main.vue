<template>
    <main>
      <div class="base-page">
        <OurSpecialties :propSpecialties="specialties" />
        <Bickford />
      </div>
    </main>
</template>

<script>
import OurSpecialties from './OurSpecialties.vue';
import Bickford from './Bickford.vue';

export default {
  name: "Main",
  components: {
    OurSpecialties,
    Bickford
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
          icon: '../assets/svg/svg-1.svg',
          title: 'Selling',
          text: 'Lorem ipsum dolor sit amet, quis consect.'
        },
        {
          icon: '../assets/svg/svg-2.svg',
          title: 'Learning',
          text: 'Lorem ipsum dolor sit amet, quis consect.'
        },
        {
          icon: '../assets/svg/svg-3.svg',
          title: 'Contact',
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
}


</style>