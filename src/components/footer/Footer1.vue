<template>
  <div>
    <div class="backg-theme-1">
      <div class="container mt-5">
        <div class="row text-light">
          <div class="col-sm">
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
          <div class="col-sm">
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
          <div class="col-sm">One of three columns</div>
        </div>
      </div>
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
  border-top: #20d3c2 solid 6px;
  border-bottom: #080c24 sol;
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
  background-color: #20d3c2 !important;
  /* border-bottom: 1px solid #20d3c2; */
  position: absolute;
  left: 100px;
  top: 12px;
}
</style>