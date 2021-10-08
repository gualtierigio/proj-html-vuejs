<template>
    <div class="page-wrap">
        <div class="container">
            <!-- title news -->
            <div class="row mb-10">
                <div class="col-12">
                    <div class="text-center">
                        <h1>Our Specialties<span class="red-dot">.</span></h1>
                        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ipsum debitis perferendis vitae.</p>
                        <div class="red-line"></div>
                    </div>
                </div>
            </div>
            <!-- img news -->
            <div class="row">
                <div v-for="(element, index) in propEvents" :key="index" class="col-4">
                    <div class="img-wrap">
                        <img :src="element.img" alt="">
                    </div>
                    <div class="d-flex when-where">
                        <i class="far fa-clock"></i>
                        <p>{{element.month}}{{element.day}},{{element.year}}</p>
                        <i class="far fa-user"></i>
                        <p>Armanda Doe</p>
                    </div>
                    <h4>{{element.businessType}}</h4>
                    <p class="space-line">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laboriosam, velit! Ullam eius quasi est inventore quidem facere.</p>
                    <h5 class="more">read more</h5>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CreativeLeader',
    props: {
        'propEvents' : Array
    }
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

.img-wrap{
    width: 100%;
    height: 400px;
    margin-bottom: 35px;
    img{
        width: 100%;
        height: 100%;
        object-fit: cover;
        background-repeat: no-repeat;
    }
}

.when-where{
    p{
        margin: 0 20px;
    }
    i{
        color: $red-color;
        font-size: 0.7rem;
        margin-bottom: 20px;
    }
}



// utilities

p{
    font-size: 0.7rem;
    font-weight: 300;
    opacity: 0.7;
    margin-bottom: 20px;
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

.mb-10{
    margin-bottom: 100px;
}

.more{
    font-size: 0.8rem;
    font-weight: bold;
    text-transform: uppercase;
}

.space-line{
    line-height: 25px;
}

</style>