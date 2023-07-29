<template>
  <div class="container">
    <div class="content d-flex justify-content-center align-items-center">
        <div class="title text-center text-dark">
            <h4 class="custom-h4 pt-2">My Portfolio</h4>
            <span>My work will prove my quality</span>
        </div>
    </div>
    <div class="row portfolio">
        <div class="col-lg-4 col-sm-6 col-md-4 d-flex justify-content-center">
            <div class="wrapper  text-white">
                <img src="../assets/img/portfolio/SiteFes.jpg" alt="img" class="img-fluid img-custom">
            </div>
        </div>
        <div class="col-lg-4 col-sm-6 col-md-4 d-flex justify-content-center">
            <div class="wrapper flex text-white">
                <img src="../assets/img/portfolio/Kiosk.jpg" alt="img" class="img-fluid img-custom">
            </div>
        </div>
        <div class="col-lg-4 col-sm-6 col-md-4 d-flex justify-content-center">
            <div class="wrapper text-white">
                <img src="../assets/img/portfolio/Olden.jpg" alt="img" class="img-fluid img-custom">
            </div>
        </div>
        
        <div class="col-lg-4 col-sm-6 col-md-4 d-flex justify-content-center">
            <div class="wrapper text-white">
                <img src="../assets/img/portfolio/founding.jpg" alt="img" class="img-fluid img-custom">
            </div>
        </div>

        <div class="col-lg-4 col-sm-6 col-md-4 d-flex justify-content-center">
            <div class="wrapper flex text-white">
                <img src="../assets/img/portfolio/auidols.jpg" alt="img" class="img-fluid img-custom">
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.container {
    max-width: 1450px;
    padding: 20px;
}

.portfolio {
    margin-bottom: 150px;
}

.img-custom {
    width: 100%;
    height: 90%;
}

.content {
    min-height: 300px;
}

.custom-h4 {
    font-weight: bolder;
}

.wrapper {
  transition: transform 0.3s ease;
  /* The element is at its default scale (1x) */
}

.wrapper:hover {
  transform: scale(1.1);
  cursor: pointer;
  box-shadow: 2px;
}


</style>