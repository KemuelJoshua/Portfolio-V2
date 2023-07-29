<template>
  <div class="container-fluid">
    <div class="row">
        <div class="col-lg-6 col-md-6 col-sm-12 col-xs-12">
            <img src="../assets/img/leadership.jpg" alt="leadership-img" class="img-fluid fit-image">
        </div>
        <div class="col-lg-6 col-md-6 col-sm-12 col-xs-12">
            <div class="content text-dark">
                <h4 class="custom-h4 pt-3">Leadership Experience.</h4>

                <div class="mt-5 mb-5">
                    <h5>LITES Organization President</h5>
                    <span>2023-2024</span>
                </div>
                <div class="mt-5 mb-5">
                    <h5>LITES Organization Vice President</h5>
                    <span>2022-2023</span>
                </div>
                <div class="mt-5 mb-5">
                    <h5>AUMMC Graphic Designer</h5>
                    <span>2021-2023</span>
                </div>
                <div class="mt-5 mb-5">
                    <h5>AUSSC Director for Graphic and Design</h5>
                    <span>2022-2023</span>
                </div>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.container-fluid {
    margin: 0px;
    padding: 0px    ;
}
@media (min-width: 767px){
    .content {
     margin: 100px;
    }
   
}
@media (max-width: 768px) {
    .content {
        padding: 10px;
    }
}

.fit-image {
  width: 100%;
  height: 100%;
  object-fit: cover; /* This will make the image cover the entire container */
}

.custom-h4 {
    font-weight: bolder;
    text-transform: uppercase;
}

h5 {
    font-weight: bolder;
}
</style>