<template>
  <div>
    <div class="overlay-container pb-5">
        <div class="background bg-primary"></div>
            <div class="greet d-flex align-items-center justify-content-center">
                <div class="content">
                <h5 class="text-center custom text-white">Hi!, I'm Kemuel Joshua Mariano. Nice to see you here.</h5>
                <p class="text-white text-center" style="font-weight: 100;">
                    Pursuing a Bachelor of Science in Information Technology. Passionate about web and mobile development since high school. Eager to make a positive impact with innovative tech solutions. Excited for the future in this field!
                </p>
                </div>
            </div>
        <div class="row d-flex justify-content-center tech-stack">
            <div class="col-xl-3 col-lg-4 col-md-5 col-sm-10 col-9 bg-white text-dark card" >
                <div class="d-flex justify-content-center align-items-start">
                    <div class="text-center">
                        <img src="../assets/img/frontend.png" 
                        height="100px" width="100px" alt="frontend" class="mx-auto d-block m-4">
                        <h4 class="m-4 custom">Frontend Development</h4>
                        <p>I like to code things from scratch, and enjoy bringing ideas to life in the browser.</p>

                        <h5 class="mt-5 text-primary">Language I speak:</h5>
                        <p class="text-dark">HTML | CSS | Javascript <br> Sass | Git</p>


                        <h5 class="mt-5 text-primary">Design Tools:</h5>
                        <h5 class="text-dark">Vue JS</h5>
                        <h5 class="text-dark">React JS</h5>
                        <h5 class="text-dark">Bootsrap 5</h5>
            
                    </div>
                </div>
            </div>
            <div class="col-lg-3 col-md-5 col-sm-10 col-9 bg-white text-dark card" >
                <div class="d-flex justify-content-center align-items-start">
                    <div class="text-center">
                        <img src="../assets/img/backend.png" 
                        height="100px" width="100px" alt="frontend" class="mx-auto d-block m-4">
                        <h4 class="m-4 custom">Backend Development</h4>
                        <p>I like to code things from scratch, and enjoy bringing ideas to life in the browser.</p>

                        <h5 class="mt-5 text-primary">Language I speak:</h5>
                        <p class="text-dark">Node JS | PHP | Java</p>


                        <h5 class="mt-5 text-primary">Development Tools:</h5>
                        <h5 class="text-dark">Express JS</h5>
                        <h5 class="text-dark">Firebase</h5>
                        <h5 class="text-dark">Amazon AWS</h5>
                        <h5 class="text-dark">Postman</h5>
                        <h5 class="text-dark">Mysql</h5>
                        <h5 class="text-dark">Google Services</h5>
                    </div>
                </div>
            </div>
            <!--
            <div class="col-lg-3 col-md-3 col-sm-4 col-xs-4 bg-white text-dark card" >
                <div class="d-flex justify-content-center align-items-start">
                    <div class="text-center m-5">
                        <img src="../assets/img/backend.png" 
                        height="100px" width="100px" alt="frontend" class="mx-auto d-block m-4">
                        <h4 class="m-4 custom">Backend Development</h4>
                        <p>I like to code things from scratch, and enjoy bringing ideas to life in the browser.</p>

                        <h5 class="mt-5 text-primary">Language I speak:</h5>
                        <p class="text-dark">Node JS | PHP | Java</p>


                        <h5 class="mt-5 text-primary">Development Tools:</h5>
                        <h5 class="text-dark">Express JS</h5>
                        <h5 class="text-dark">Firebase</h5>
                        <h5 class="text-dark">Amazon AWS</h5>
                        <h5 class="text-dark">Postman</h5>
                        <h5 class="text-dark">Mysql</h5>
                        <h5 class="text-dark">Google Services</h5>
            
                    </div>
                </div>
            </div>-->
        </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.tech-stack {
    min-height: 800px;
}
.overlay-container {
  position: relative;
}
.custom {
    font-weight: bold;
}

.background {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 600px; 
  z-index: 0; 
}

.card {
  border-radius: 2px;
}

.greet {
  position: relative;
  height: 350px;
  z-index: 1;
}

@media (max-width: 1001px) {
    .background  {
        height: 700px; 
    }
    .greet {
          height: 350px;
    }
}

@media (max-width: 576px) {
    .background  {
        height: 500px; 
    }

    .greet {
          height: 400px;
    }
}

.content {
  max-width: 800px;
}
</style>