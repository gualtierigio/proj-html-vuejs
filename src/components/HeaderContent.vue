<template>
  <div class="d-flex" id="header-content-wrap">
        <div class="arrows">
          <i class="fas fa-long-arrow-alt-left"></i>
        </div>
        <div class="container d-flex">
            <div class="row">
                <div class="col-12 col-lg-7 d-flex align-items-center">
                    <div class="our-team__content">
                        <h1>Our team<span class="red-dot">.</span></h1>
                        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Neque delectus deserunt recusandae tempore quaerat quod.</p>
                        <div class="buttons d-flex">
                            <div class="button-custom d-flex">
                                <div class="text-button">
                                    <h6>read more</h6>
                                </div>
                                <div class="arrow-button">
                                    <i class="fas fa-long-arrow-alt-right"></i>
                                </div>
                            </div>
                            <div class="button-custom left-button d-flex">
                                <div class="text-button">
                                    <h6>purchase</h6>
                                </div>
                                <div class="arrow-button-left">
                                    <i class="fas fa-long-arrow-alt-right"></i>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
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
    width: 100%;
    height: 65vh;
    min-width: 620px;
}

.arrows{
    display: flex;
    align-items: center;
    height: 100%;
    width: 60px;
    padding: 10px;
    i{
        font-size: 40px;
    }
}

.our-team__content{
    padding: 0 20px;
    h1{
        font-size: 5.5rem;
        font-weight: bold;
        margin-bottom: 40px;
    }
    p{
        font-size: 1.2rem;
        color: $gray-text-color-1;
        margin-bottom: 40px;
    }
}

.button-custom{
    height: 60px;
    width: 200px;
    background-color: $total-white;
    padding: 10px 0;
    h6{
        text-transform: uppercase;
        font-size: 0.8rem;
        font-weight: bold;
        margin-bottom: 0;
    }
}

.left-button{
    background-color: $red-color;
    margin-left: 20px;
    color: $total-white;
}

.text-button,.arrow-button,.arrow-button-left{
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    i{
        font-size: 1.6rem;
    }
}

.text-button{
    width: 100%;
}

.arrow-button-left,.arrow-button{
    width: 40%;
}

.arrow-button{
    border-left: 1px solid $total-black;
}

.arrow-button-left{
    border-left: 1px solid $total-white;
}


.red-dot{
  color: $red-color;
}


</style>