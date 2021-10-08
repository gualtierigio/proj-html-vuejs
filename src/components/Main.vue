<template>
    <main>
      <div class="base-page">
        <OurSpecialties :propSpecialties="specialties" />
        <img class="svg-bg" src="../assets/svg/svg-4.svg" alt="svg background">
        <Bickford />
      </div>
      <Events :propEvents="events"/>
      <div class="position-relative">
        <CreativeLeader />
        <img class="svg-bg-left" src="../assets/svg/svg-4.svg" alt="svg background">
        <div id="news">
          <LatestNews :propEvents="events"/>
        </div>
      </div>
    </main>
</template>

<script>
import OurSpecialties from './OurSpecialties.vue';
import Bickford from './Bickford.vue';
import Events from './Events.vue';
import CreativeLeader from './CreativeLeader.vue';
import LatestNews from './LatestNews.vue';

export default {
  name: "Main",
  components: {
    OurSpecialties,
    Bickford,
    Events,
    CreativeLeader,
    LatestNews
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
          where: 'Mealbourne Coaching',
          position: 'Cambrige, MA 02138,USA',
          day: '7',
          month: 'Jan',
          time: '9:00 am - 5:00 pm',
          year: '2022',
          businessType: 'Next investment'
        },
        {
          where: 'New York Coaching',
          position: 'Cambrige, MA 02138,USA',
          day: '11',
          month: 'Jan',
          time: '9:00 am - 5:00 pm',
          year: '2022',
          businessType: 'Team Building'
        },
        {
          where: 'London Coaching',
          position: 'Cambrige, MA 02138,USA',
          day: '21',
          month: 'Jan',
          time: '9:00 am - 5:00 pm',
          year: '2022',
          businessType: 'New Business Day'
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

#news{
  background-color: $white-color-5;
  padding: 50px 0;
}

.svg-bg,.svg-bg-left{
  position: absolute;
  filter: invert(9%) sepia(5%) saturate(21%) hue-rotate(357deg) brightness(88%) contrast(91%);
}

.svg-bg{
  right: 100px;
  top: 50%;
}

.svg-bg-left{
  left: 100px;
  top: 30%;
}


</style>