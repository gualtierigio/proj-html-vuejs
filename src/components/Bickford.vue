<template>
    <div class="page-wrap">
        <div class="img-container">
            <img src="../assets/img/h1-img-01.jpg" alt="interview image">
            <div class="change-img d-flex align-items-center justify-content-around">
                <img class="rotate" src="../assets/svg/svg-6.svg" alt="&larr;">
                <img src="../assets/svg/svg-6.svg" alt="&larr;">
            </div>
        </div>
        <div class="bickford-comment">
            <h1>Jason Bickford</h1>
            <h6>Founder and Executive Director</h6>
            <div class="red-line"></div>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis odio, in vero esse fugiat molestias libero, possimus tempora totam sint architecto quae corporis...</p>
            <div class="socials d-flex">
            <div class="social-custom">
                <i class="fab fa-twitter"></i>
            </div>
            <div class="social-custom">
                <i class="fab fa-facebook-f"></i>
            </div>
            <div class="social-custom">
                <i class="fab fa-linkedin-in"></i>
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
  margin: 100px auto 0 auto;
  padding-bottom: 100px;
  position: relative;
}

// img part

.img-container{
    height: 600px;
    width: 720px;
    position: relative;
    img{
        width: 100%;
        height: 100%;
        object-fit: cover;
    }
}

.change-img{
    width: 140px;
    height: 80px;
    background-color: $red-color;
    position: absolute;
    bottom: 0;
    left: 0;
    img{
        width: 40px;
        height: 40px;
    }
    img:hover{
        opacity: 0.6;
        cursor: pointer;
    }
    img.rotate{
            transform: rotate(180deg);
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
    padding: 100px 90px 100px 60px;
    h6{
    color: $black-color-1;
    font-size: 0.7rem;
    opacity: 0.7;
    }
    p{
    color: $black-color-1;
    font-weight: 300;
    font-size: 0.8rem;
    margin-bottom: 30px;
    opacity: 0.7;
    }
}

// specific implementation

.social-custom{
  width: 25px;
  height: 25px;
  background-color: $red-color;
  border-radius: 50%;
  margin-right: 10px;
  position: relative;
  i{
    color: $total-white;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
  }
}

.social-custom:hover{
    opacity: 0.6;
    cursor: pointer;
}

.red-line{
  width: 100px;
  height: 2px;
  background-color: $red-color;
  margin: 25px 0;
}

.red-dot{
  color: $red-color;
}

</style>