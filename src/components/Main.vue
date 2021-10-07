<template>
    <main>
      <div class="base-page">
        <OurSpecialties />
      </div>
    </main>
</template>

<script>
import OurSpecialties from './OurSpecialties.vue';

export default {
  name: "Main",
  components: {
    OurSpecialties
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