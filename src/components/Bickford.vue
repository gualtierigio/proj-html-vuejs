<template>
    <div class="page-wrap">

    </div>
</template>

<script>
export default {
    name: 'Bickford',
}
</script>

<style scoped lang="scss">
@import '../style/general.scss';
@import '../style/variables.scss';

.page-wrap{
  width: 70%;
  margin: 0 auto;
  border: 1px solid red;
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