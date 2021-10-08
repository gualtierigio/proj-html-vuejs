<template>
    <div class="page-wrap">
        <div class="img-container">
            <img src="../assets/img/h1-img-01.jpg" alt="interview image">
        </div>
        <div class="bickford-comment">

        </div>

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
  margin: 100px auto 0 auto;
  padding-bottom: 100px;
  position: relative;
}

.img-container{
    height: 600px;
    width: 720px;
    img{
        width: 100%;
        height: 100%;
        object-fit: cover;
    }
}

// text right part

.bickford-comment{
    width: 700px;
    height: 500px;
    position: absolute;
    right: 0;
    top: 50px;
    background-color: $total-white;
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