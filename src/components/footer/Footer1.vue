<template>
  <div>
    <!-- position-relative  d-flex-->
    <div class="backg-theme-1 position-relative">
      <!-- mydotted -->
      <div class="container mt-5">
        <!-- justify-content-center -->
        <div class="row text-light m-0">
          <div class="col">
            <div class>
              <Logo2></Logo2>
            </div>

            <div class="mt-4">
              <p
                class="text-color-light mt-2 fz-14"
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
                <div class="instagramprimary rounded">
                  <i class="fab fa-instagram fa-2x"></i>
                </div>
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

      <!-- back to top -->
      <button class="btn btn-backToTop">
        <img src="@/assets/ArrowUp.png" alt />
      </button>
      <!--  -->
    </div>

    <div class="backg-theme-2">
      <div class="container ">
        <!-- mt-2 -->
        <div class="pt-1 pb-1">
          <!-- align-items-center justify-content-center justify-content-around -->
          <div class="row  justify-content-between align-items-center">
            <div class="col-12 col-lg-5">
              <div class="row p-2">
                <div class="col ">
                  <p class="text-light m-0">&copy; copyright 2020 KenKata</p>
                  
                </div>
              </div>
            </div>
            <div class="col-12 col-lg-5">
              <!-- justify-content-center -->
              <div class="row justify-content-around p-2">
                <div class="col-3 col-lg-2 p-1">
                  <img src="@/assets/payment_master.png" />
                </div>
                <div class="col-3 col-lg-2 p-1">
                  <img src="@/assets/payment_paypal.png" />
                </div>
                <div class="col-3 col-lg-2 p-1">
                  <img src="@/assets/payment_visa.png" />
                </div>
                <div class="col-3 col-lg-2 p-1">
                  <img src="@/assets/payment_Payoneer.png" />
                </div>
                <div class="col-3 col-lg-2 p-1">
                  <img src="@/assets/payment_discover.png" />
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
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
.mydotted {
  border: 1px dotted black;
}
.mydottedw {
  border: 1px dotted white;
}

.backg-theme-1 {
  /*  #0E153D */
  background-color: #0e153d;
  border-top: var(--primaryColor) solid 6px;
  min-height: 100px;
}
.backg-theme-2 {
  /*  #0E153D */
  background-color: #080c24;
  /* min-height: 80px; */
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
.instagramprimary {
  display: flex;
  height: 78px;
  width: 78px;
  background-color: var(--primaryColor) !important;
  /* border-radius: ; */
  margin: 0.5rem;
  /* padding: 20px; */
  justify-content: center;
  align-items: center;
}

.btn-backToTop {
  position: absolute;
  right: 5%;
  top: 5%;
  background-color: var(--primaryColor) !important;
  z-index: 2;
}
</style>