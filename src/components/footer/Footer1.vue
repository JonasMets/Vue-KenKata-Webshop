<template>
  <div>
    <div class="backg-theme-1 d-flex">
      <div class="container mt-5">
        <div class="row text-light">
          <div class="col">
            <div class>
              <Logo2></Logo2>
            </div>

            <div class="mt-4">
              <p
                class="text-color-light mt-2"
              >Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent enim quam, ullamcorper vel tellus vitae, tempus fringilla lectus. Donec maximus justo eu nisl convallis iaculis. Aenean laoreet.</p>
            </div>
            <div class>
              <div class="position-relative d-flex">
                <p class>Follow Us</p>
                <p class="myline1"></p>
              </div>

              <div class="row">
                <a class="nav-link text-light" href="#">
                  <i class="fab fa-facebook-f text-color-primary"></i>
                </a>

                <a class="nav-link text-light" href="#">
                  <i class="fab fa-twitter text-color-primary"></i>
                </a>

                <a class="nav-link text-light" href="#">
                  <i class="fab fa-instagram text-color-primary"></i>
                </a>

                <a class="nav-link text-light" href="#">
                  <i class="fab fa-pinterest-p"></i>
                </a>

                <a class="nav-link text-light" href="#">
                  <i class="fab fa-youtube text-color-primary"></i>
                </a>
              </div>
            </div>
          </div>
          <div class="col">
            <h5 class="text-color-primary text-style-head">CONTACTINFO</h5>
            <div>
              <p class="text-color-primary">Adress:</p>
              <p>Solna Business Park</p>
              <p>Feni-2500, Stockholm</p>
            </div>
            <div>
              <p class="text-color-primary">Phone:</p>
              <p>+08-123456789</p>
              <p>+08-123456789</p>
            </div>
            <div>
              <p class="text-color-primary">Email:</p>
              <p>support@website.com</p>
              <p>info@website.com</p>
            </div>
          </div>
          <div class="col">
            <h5 class="text-color-primary text-style-head">USEFUL LINKS</h5>
            <div>
              <a class="nav-link text-light usefullinksstyle" href="#">Privacy Policy</a>
              <a class="nav-link text-light usefullinksstyle" href="#">Terms & Conditions</a>
              <a class="nav-link text-light usefullinksstyle" href="#">Contact Us</a>
              <a class="nav-link text-light usefullinksstyle" href="#">Our Sitemap</a>
              <a class="nav-link text-light usefullinksstyle" href="#">Latest News</a>
              <a class="nav-link text-light usefullinksstyle" href="#">Returns</a>
            </div>
          </div>
          <div class="col">
            <h5 class="text-color-primary text-style-head">RECENT INSTAGRAM</h5>
            <!-- <div class="row justify-content-between">
              <div class="col-12">
                <a href="#" class>
                  <div class="instagramgrey rounded"></div>
                </a>
              </div>
              <div class="col-12">
                <a href="#" class>
                  <div class="instagramgrey rounded"></div>
                </a>
              </div>
              <div class="col-12">
                <a href="#" class>
                  <div class="instagramgrey rounded"></div>
                </a>
              </div>
            </div>-->

            <div class="row justify-content-between">
              <div class="col-5 col-lg-4">
                <div class="instagramgrey rounded"></div>
              </div>
              <div class="col-5 col-lg-4">
                <div class="instagramgrey rounded"></div>
              </div>
              <div class="col-5 col-lg-4">
                <div class="instagramgrey rounded"></div>
              </div>
              <div class="col-5 col-lg-4">
                <div class="instagramgrey rounded"></div>
              </div>
              <div class="col-5 col-lg-4">
                <div class="instagramgrey rounded"></div>
              </div>
              <div class="col-5 col-lg-4">
                <div class="instagramgrey rounded"></div>
              </div>
              <div class="col-5 col-lg-4">
                <div class="instagramgrey rounded"></div>
              </div>
              <div class="col-5 col-lg-4">
                <div class="instagramgrey rounded"></div>
              </div>
              <div class="col-5 col-lg-4">
                <div class="instagramgrey rounded"></div>
              </div>
            </div>
          </div>
        </div>
        <!-- end row -->
      </div>

      <!--  -->
      <!-- <div class="row"> -->
      <!-- <div class="col"> -->
      <!-- d-flex justify-content-end -->
      <div class="mt-4 mr-5">
        <button class="btn btn-backToTop">
          <img src="@/assets/ArrowUp.png" alt />
        </button>
      </div>
      <!-- </div> -->
      <!-- </div> -->
    </div>

    <div class="backg-theme-2">
      <div class="container"></div>
    </div>
  </div>
</template>

<script>
import Logo2 from "@/components/logo/Logo2";

export default {
  components: {
    Logo2,
  },
};
</script>

<style scoped>
.backg-theme-1 {
  /*  #0E153D */
  background-color: #0e153d;
  border-top: var(--primaryColor) solid 6px;
  min-height: 100px;
}
.backg-theme-2 {
  /*  #0E153D */
  background-color: #080c24;
  min-height: 80px;
}

.text-color-primary {
  color: var(--primaryColor);
}
.text-style-head {
  font-size: 18px;
}

.myline1 {
  margin: 0;
  width: 39px;
  height: 1px;
  background-color: var(--primaryColor) !important;
  position: absolute;
  left: 100px;
  top: 12px;
}

.usefullinksstyle {
  padding: 0;
  margin: 1rem 0;
}
.usefullinksstyle:hover {
  color: var(--primaryColor) !important;
  text-decoration: underline;
}

.instagramgrey {
  height: 78px;
  width: 78px;
  background-color: #cccccc;
  /* border-radius: ; */
  margin: 0.5rem;
  /* padding: 20px; */
}

.btn-backToTop {
  background-color: var(--primaryColor) !important;
}
</style>