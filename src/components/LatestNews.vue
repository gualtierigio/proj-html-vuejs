<template>
    <div class="page-wrap">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <div class="text-center">
                        <h1>Our Specialties<span class="red-dot">.</span></h1>
                        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ipsum debitis perferendis vitae.</p>
                        <div class="red-line"></div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CreativeLeader',
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




// utilities

p{
    font-size: 0.7rem;
    font-weight: 300;
    opacity: 0.7;
    margin-bottom: 20px;
    line-height: 25px;
}

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