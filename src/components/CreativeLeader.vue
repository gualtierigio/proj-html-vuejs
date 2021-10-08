<template>
    <div class="page-wrap">
        <div class="container">
            <div class="row">
                <div class="col-6">
                    <h3>Creative Leader<span class="red-dot">.</span></h3>
                    <div class="red-line"></div>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt nemo illo quo culpa consectetur laborum ullam quam esse magni quia maiores, nostrum natus, iure eaque numquam perferendis, porro doloremque blanditiis?</p>
                    <h5 class="more">read more</h5>
                </div>
            </div>
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
  padding: 100px 0;
  margin: 0 auto;
}

.red-line{
  width: 100px;
  height: 2px;
  background-color: $red-color;
  margin: 15px 0;
}

.more{
    font-size: 0.8rem;
    font-weight: bold;
    text-transform: uppercase;
}

p{
    font-size: 0.7rem;
    font-weight: 300;
    opacity: 0.7;
    margin-bottom: 20px;
    line-height: 25px;
}

.red-dot{
  color: $red-color;
}

</style>