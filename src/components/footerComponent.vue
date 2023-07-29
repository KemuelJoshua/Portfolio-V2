<template>
  <footer class="bg-white2">
    <div class="d-flex align-items-center footer-content">
        <div class="container">
            <div class="row">
                <div class="col-lg-12">
                    <div class="footer-top">
                        <div class="content">
                            <span>Starting a project!</span>
                            <h4 class="custom-h4 pt-2">Contact Me!</h4>
                        </div>
                    </div>
                </div>
            </div>
            <div class="row d-flex align-items-center">
                <div class="col-md-6 col-lg-3 col-sm-6 mt-5 mb-3 ">
                    <h5>Present Address</h5>
                    <a>Caritas RD Calzada </a><br>
                    <a>Tipas Taguig City</a>
                </div>
                <div class="col-md-6 col-lg-3 col-sm-6 mt-5 mb-3 ">
                    <h5>Home Address</h5>
                    <a>Caritas RD Calzada </a><br>
                    <a>Tipas Taguig City</a>
                </div>
                <div class="col-md-6 col-lg-3 col-sm-6 mt-5 mb-3 ">
                    <h5>Contact</h5>
                    <a>kemueljoshuamariano</a><br>
                    <a>+639-29870 4337</a>
                </div>
                <div class="col-md-6 col-lg-3 col-sm-6 mt-5 mb-3 ">
                    <h5>Social Media</h5>
                    <a>FB : kemuel.mariano28</a><br>
                    <a>IG : kemwellss</a>
                </div>
            </div>
        </div>
    </div>
    <div class="copyright bg-white d-flex justify-content-center align-items-center">
        <span>@2023 KJM. All Rights Reserved.</span>
    </div>
  </footer>
</template>

<script>
export default {

}
</script>

<style scoped>
.container {
    max-width: 1400px;
    padding: 10px;
}
footer {
    color: black;
}

span {
    font-weight: 100;
}
h5 {
    font-weight: bold;
}

.footer-content {
    min-height: 550px;
    max-height: 700px;
}
a {
    font-weight: 100;
}
.copyright {
    height: 70px;
    width: 100%;
}
.content {
    height: 200px;
    max-height: 350px;
}
h4 {
    font-weight: bolder;
}

@media (max-width: 991px) {
    .content {
        height: 100px;
    }
}
</style>