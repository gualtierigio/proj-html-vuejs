<template>
    <div class="bg-img">
        <div class="page-wrap">
        </div>
    </div>
</template>

<script>
export default {
    name: 'Events',
}
</script>

<style scoped lang="scss">
@import '../style/general.scss';
@import '../style/variables.scss';

.page-wrap{
  width: 70%;
  margin: 0 auto;
}

.bg-img{
    width: 100%;
    height: 100vh;
    background-image: url(../assets/img/h1-img-09.jpg);
    background-size: cover;
    background-repeat: no-repeat;
}



</style>