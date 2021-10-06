<template>
  <div class="d-flex" id="header-content-wrap">
        <div class="arrows">
          <i class="fas fa-long-arrow-alt-left"></i>
        </div>
        <div class="our-team"></div>
        <div class="arrows">
          <i class="fas fa-long-arrow-alt-right"></i>
        </div>
  </div>
</template>

<script>
export default {
    name: 'HeaderContent',
}
</script>

<style lang="scss" scoped>
@import '../style/general.scss';
@import '../style/variables.scss';

#header-content-wrap{
    margin-top: 100px;
    border: 1px solid red;
    width: 100%;
    height: 65vh;
}

.arrows{
    display: flex;
    align-items: center;
    height: 100%;
    width: 60px;
    padding: 10px;
    border: 1px solid red;
    i{
        font-size: 40px;
    }
}

.our-team{
    height: 100%;
    width: calc(100% - 120px);
    border: 1px solid red;
}


</style>