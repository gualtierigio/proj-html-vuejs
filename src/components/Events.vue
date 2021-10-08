<template>
    <div class="bg-img d-flex align-items-center">
        <div class="page-wrap">
            <div id="events-wrapper">
                <div class="events-title">
                    <h2>Upcoming Events</h2>
                </div>
                <div class="appointment d-flex">
                    <div class="data">
                        <h6>07</h6>
                        <p>Jan,2022</p>
                    </div>
                    <div class="when-where">
                        <h4>Melbourne Coaching</h4>
                        <div class="d-flex">
                            <i class="far fa-clock"></i>
                            <p>9:00 am - 5:00 pm, Jan 7,2022</p>
                        </div>
                        <div class="d-flex">
                            <i class="fas fa-map-marker-alt"></i>
                            <p>Cambrige, MA 02138,USA</p>
                        </div>
                        <h5>read more</h5>
                    </div>
                </div>
            </div>
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

#events-wrapper{
    width: 40%;
    height: 500px;
}

.events-title{
    width: 100%;
    height: 70px;
    padding: 18px 35px;
    background-color: $total-white;
    h2{
        font-size: 1.4rem;
        font-weight: bold;
    }
}

.appointment{
    width: 100%;
    height: 200px;
    background-color: $white-color-5;
    border-bottom: 1px solid gray;
    padding: 30px;
}

.appointment:hover{
    background-color: $total-white;
    cursor: pointer;
}

.data{
    background-color: $red-color;
    padding: 5px;
    text-align: center;
    color: $total-white;
    margin-right: 20px;
    height: 50%;
    h6{
        font-weight: bold;
        font-size: 1.4rem;
    }
    p{
        font-size: 0.8rem;
    }
}

.when-where{
    h4{
        font-size: 1.2rem;
        font-weight: bold;
        padding-bottom: 20px;
    }
    p{
        font-size: 0.7rem;
        font-weight: 300;
    }
    i{
        color: $red-color;
        margin-right: 20px;
    }
    h5{
        font-size: 0.8rem;
        font-weight: bold;
        text-transform: uppercase;
    }
}



</style>