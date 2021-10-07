<template>
  <div class="d-flex" id="header-content-wrap">
        <div class="arrows">
          <i class="fas fa-long-arrow-alt-left"></i>
        </div>
        <div class="our-team d-flex align-items-end">
            <div class="our-team__content">
                <h1>Our team<span class="red-dot">.</span></h1>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Voluptatum iste, reprehenderit ipsam assumenda aliquid architecto inventore possimus ut? Nulla quis quam illo reprehenderit. Neque delectus deserunt recusandae tempore quaerat quod!</p>
                <div class="buttons d-flex">
                    <div class="button-custom d-flex">
                        <div class="text-button">
                            <h6>read more</h6>
                        </div>
                        <div class="arrow-button">
                            <i class="fas fa-long-arrow-alt-right"></i>
                        </div>
                    </div>
                    <div class="button-custom d-flex">
                        <div class="text-button">
                            <h6>read more</h6>
                        </div>
                        <div class="arrow-button">
                            <i class="fas fa-long-arrow-alt-right"></i>
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
    border: 1px solid red;
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

.our-team__content{
    width: 80%;
    height: 70%;
    padding: 0 20px;
    border: 1px solid red;
    h1{
        font-size: 5.5rem;
        font-weight: bold;
    }
    p{
        font-size: 0.8rem;
        color: $gray-text-color-1;
    }
}

.buttons{
    padding: 0 20px;
    border: 1px solid red;
}

.button-custom{
    height: 60px;
    width: 200px;
    margin-left: 20px;
    background-color: $total-white;
    padding: 10px 0;
    h6{
        text-transform: uppercase;
        font-size: 0.8rem;
        font-weight: bold;
    }
}

.text-button,.arrow-button{
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    i{
        font-size: 2rem;
    }
}

.text-button{
    width: 100%;
}

.arrow-button{
    border-left: 1px solid $total-black;
    width: 40%;
}

.red-dot{
  color: $red-color;
}


</style>