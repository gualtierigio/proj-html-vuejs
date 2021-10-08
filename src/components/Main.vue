<template>
    <main>
      <div class="base-page">
        <OurSpecialties :propSpecialties="specialties" />
        <img class="svg-bg" src="../assets/svg/svg-4.svg" alt="svg background">
        <Bickford />
      </div>
      <Events />
    </main>
</template>

<script>
import OurSpecialties from './OurSpecialties.vue';
import Bickford from './Bickford.vue';
import Events from './Events.vue';

export default {
  name: "Main",
  components: {
    OurSpecialties,
    Bickford,
    Events
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
      ],
      events: [
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
  background-color: $white-color-6;
  position: relative;
}

.svg-bg{
  position: absolute;
  right: 100px;
  top: 50%;
  filter: invert(9%) sepia(5%) saturate(21%) hue-rotate(357deg) brightness(88%) contrast(91%);
}


</style>