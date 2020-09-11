<template>
  <div id="topnav">
    <div class="container">
      <!-- <Language></Language> -->

      <!-- <Currency></Currency> -->

      <nav class="navbar navbar-expand-lg navbar-light">
        <!-- <a class="navbar-brand" href="#">Navbar</a> -->
        <!-- <ul class="navbar-nav">
          <li class="nav-item">
            <Language></Language>
          </li>
          <li class="nav-item">
            <Currency></Currency>
          </li>
        </ul>-->

        <button
          class="navbar-toggler ml-auto"
          type="button"
          data-toggle="collapse"
          data-target="#navbarSupportedContent1"
          aria-controls="navbarSupportedContent1"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>

        <div class="collapse navbar-collapse" id="navbarSupportedContent1">

          <ul class="navbar-nav">
            <li class="nav-item">
              <Language></Language>
            </li>
            <li class="nav-item border-right">
              <Currency></Currency>
            </li>
          </ul>

          <ul class="navbar-nav ml-auto">
            <li class="nav-item active border-right">
              <!-- <span class="sr-only">(current)</span> -->
              <a class="nav-link text-light" href="#">Newsletter</a>
            </li>
            <li class="nav-item border-right">
              <a class="nav-link text-light" href="#">ContactUs</a>
            </li>
            <li class="nav-item border-right">
              <a class="nav-link text-light" href="#">FAQs</a>
            </li>

            <!-- social media -->
            <div>
              <ul class="navbar-nav ml-auto">
                <li class="nav-item">
                  <a class="nav-link text-light" href="#">
                    <i class="fab fa-facebook-f"></i>
                  </a>
                </li>
                <li class="nav-item">
                  <a class="nav-link text-light" href="#">
                    <i class="fab fa-twitter"></i>
                  </a>
                </li>
                <li class="nav-item">
                  <a class="nav-link text-light" href="#">
                    <i class="fab fa-instagram"></i>
                  </a>
                </li>
                <li class="nav-item">
                  <a class="nav-link text-light" href="#">
                    <i class="fab fa-pinterest-p"></i>
                  </a>
                </li>
                <li class="nav-item">
                  <a class="nav-link text-light" href="#">
                    <i class="fab fa-youtube"></i>
                  </a>
                </li>
                <!--  -->
              </ul>
            </div>

            <!-- <li class="nav-item dropdown">
        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
          Dropdown
        </a>
        <div class="dropdown-menu" aria-labelledby="navbarDropdown">
          <a class="dropdown-item" href="#">Action</a>
          <a class="dropdown-item" href="#">Another action</a>
          <div class="dropdown-divider"></div>
          <a class="dropdown-item" href="#">Something else here</a>
        </div>
            </li>-->
            <!-- <li class="nav-item">
        <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
            </li>-->
          </ul>
          <!-- <form class="form-inline my-2 my-lg-0">
      <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
      <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
          </form>-->
        </div>
      </nav>
    </div>
  </div>
</template>

<script>
import Language from "@/components/selectlanguage/Language";
import Currency from "@/components/selectcurrency/Currency";

export default {
  components: {
    //
    Language,
    Currency,
  },
};
</script>

<style scoped>
#topnav {
  background-color: #20d3c2;
  /* height: 40px; */
}
</style>