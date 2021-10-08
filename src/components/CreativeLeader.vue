<template>
    <div class="page-wrap">
        <div class="container">
            <div class="row gx-5">
                <div class="col-6">
                    <h3>Creative Leader<span class="red-dot">.</span></h3>
                    <div class="red-line static"></div>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt nemo illo quo culpa consectetur laborum ullam quam esse magni quia maiores, nostrum natus, iure eaque numquam perferendis, porro doloremque blanditiis?</p>
                    <h5 class="more">read more</h5>
                </div>
                <div class="col-6 data-percent">
                    <div class="mb-4">
                        <div class="d-flex justify-content-between">
                            <h6>Mentorship</h6>
                            <h6>78%</h6>
                        </div>
                        <div class="red-line percent mentorship"></div>
                        <div class="full-percent"></div>
                    </div>
                    <div class="mb-4">
                        <div class="d-flex justify-content-between">
                            <h6>Education</h6>
                            <h6>95%</h6>
                        </div>
                        <div class="red-line percent education"></div>
                        <div class="full-percent"></div>
                    </div>
                    <div class="mb-4">
                        <div class="d-flex justify-content-between">
                            <h6>Learning</h6>
                            <h6>65%</h6>
                        </div>
                        <div class="red-line percent learning"></div>
                        <div class="full-percent"></div>
                    </div>
                    <div>
                        <div class="d-flex justify-content-between">
                            <h6>Motivation</h6>
                            <h6>83%</h6>
                        </div>
                        <div class="red-line percent motivation"></div>
                        <div class="full-percent"></div>
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

.red-line{
  background-color: $red-color;
}

.static{
    width: 100px;
    margin: 15px 0;
    height: 2px;
}

.data-percent{
    padding: 0 80px;
}

// red line in percent

.mentorship{
    width: 78%;
}

.education{
    width: 95%;
}

.learning{
    width: 65%;
}

.motivation{
    width: 83%;
}

.percent{
    height: 4px;
}

.full-percent{
    opacity: 0.3;
    width: 100%;
    height: 1px;
    background-color: $black-color;
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