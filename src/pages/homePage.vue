<template>
      <div class="home">
        <div class="vh-100 container d-flex align-items-center" >
          <div class="container d-flex ">
            <div class="row justify-content-center text-center">
              <img src="../assets/img/myicon.png" alt="logo" class="img-fluid img-icon">
              <h1 class="text-white custom-h1">SOFT. DEVELOPER</h1>
              <p class=" text-dark">Coding with Coffee is my life.</p>
              <div class="col-12">
                <a href="#footer"  class="btn btn-support">Contact</a>
              </div>
            </div>
          </div>
        </div>
      </div>
  </template>
  
  <script>
  // @ is an alias to /src
  
  export default {
    name: 'HomeView',
    components: {},
  };
  </script>
  
  <style scoped>
   .home {
      background-image: url('../assets/img/HomeBG2.jpg');
      background-size: cover;
      background-repeat: no-repeat;
    }
  
    .custom-h1 {
      font-weight: bolder;
    }
    p {
      max-width: 800px;
      text-shadow: 1px;
    }
  .img-icon {
    height: 500px;
    width: auto;
  }
  .btn-support {
    padding: 25px,  10px, 10px, 25px;
    border-radius: 25px;
  }
  </style>
  