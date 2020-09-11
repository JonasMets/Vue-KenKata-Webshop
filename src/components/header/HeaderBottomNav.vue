
<template>
  <div class="border-top">
    <div class="container">
      <!-- bg-light -->
      <nav class="navbar navbar-expand-lg navbar-light">
        <!-- <a class="navbar-brand" href="#">Navbar</a> -->

        <!-- Example split danger button -->
        <div class="btn-group align-items-center myBrowseBtn">
          <div class="myBrowseBtn p-2">
            <img src="../../assets/Hamburgermenu.png" alt="">
          </div>

          <button type="button" class="btn myBrowseBtn">Browse Categories</button>
          <!-- dropdown-toggle -->
          <button
            type="button"
            class="btn myBrowseBtn  dropdown-toggle-split"
            data-toggle="dropdown"
            aria-haspopup="true"
            aria-expanded="false"
          >
          <!-- Toggle Dropdown -->
            <span class="sr-only"></span>
            <!-- <i class="fas fa-chevron-down"></i> -->
            <img src="../../assets/chevrondown.png" alt="">
          </button>
          <div class="dropdown-menu">
            <a class="dropdown-item" href="#">Category X</a>
            <a class="dropdown-item" href="#">Category X</a>
            <a class="dropdown-item" href="#">Category X</a>
            <div class="dropdown-divider"></div>
            <a class="dropdown-item" href="#">Category X</a>
          </div>
        </div>

        <button
          class="navbar-toggler"
          type="button"
          data-toggle="collapse"
          data-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>

        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav mr-auto">
            <li class="nav-item ">
              <a class="nav-link" href="/">
                Home
                <!-- <span class="sr-only">(current)</span> -->
              </a>
            </li>
            <!-- <li class="nav-item">
              <a class="nav-link" href="#">Shop</a>
            </li> -->
            <li class="nav-item dropdown">
              <!-- dropdown-toggle -->
              <a
                class="nav-link "
                href="#"
                id="navbarDropdown"
                role="button"
                data-toggle="dropdown"
                aria-haspopup="true"
                aria-expanded="false"
              >Shop
              <img src="../../assets/chevrondown2.png" alt="">
              </a>
              <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                <a class="dropdown-item" href="#">Shop X</a>
                <a class="dropdown-item" href="#">Shop X</a>
                <div class="dropdown-divider"></div>
                <a class="dropdown-item" href="#">Shop X</a>
              </div>
            </li>
            <li class="nav-item dropdown">
              <!-- dropdown-toggle -->
              <a
                class="nav-link "
                href="#"
                id="navbarDropdown"
                role="button"
                data-toggle="dropdown"
                aria-haspopup="true"
                aria-expanded="false"
              >Products
              <img src="../../assets/chevrondown2.png" alt="">
              </a>
              <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                <a class="dropdown-item" href="#">Products X</a>
                <a class="dropdown-item" href="#">Products X</a>
                <div class="dropdown-divider"></div>
                <a class="dropdown-item" href="#">Products X</a>
              </div>
            </li>
            <li class="nav-item dropdown">
              <!-- dropdown-toggle -->
              <a
                class="nav-link "
                href="#"
                id="navbarDropdown"
                role="button"
                data-toggle="dropdown"
                aria-haspopup="true"
                aria-expanded="false"
              >Categories
              <img src="../../assets/chevrondown2.png" alt="">
              </a>
              <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                <a class="dropdown-item" href="#">Categorie X</a>
                <a class="dropdown-item" href="#">Categorie X</a>
                <div class="dropdown-divider"></div>
                <a class="dropdown-item" href="#">Categorie X</a>
              </div>
            </li>
            <li class="nav-item dropdown">
              <!-- dropdown-toggle -->
              <a
                class="nav-link "
                href="#"
                id="navbarDropdown"
                role="button"
                data-toggle="dropdown"
                aria-haspopup="true"
                aria-expanded="false"
              >Pages
              <img src="../../assets/chevrondown2.png" alt="">
              </a>
              <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                <!--  -->
                <router-link to="/about" class="nav-link">About Us</router-link>
                <a class="dropdown-item" href="#">Page X</a>
                <a class="dropdown-item" href="#">Page X</a>
                <div class="dropdown-divider"></div>
                <a class="dropdown-item" href="#">Page X</a>
              </div>
            </li>
            <li class="nav-item ">
              <a class="nav-link" href="#">
                Blog
                <!-- <span class="sr-only">(current)</span> -->
              </a>
            </li>
            <!-- <li class="nav-item">
              <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
            </li> -->
          </ul>

          <button class="btn badge badge-pill badge-primary mybadgestyle1">SPECIAL OFFER</button>
        </div>
      </nav>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.mybadgestyle1 {
  background-color: #20d3c2 !important;
  color: #ffffff;
  /* padding-left: 0.5rem; */
  /* padding-right: 0.5rem; */
  padding: 0.4rem 0.8rem;
}

.myBrowseBtn {
  background-color: #20d3c2 !important;
  color: #ffffff;
}


/* .myBrowseBtn-toggler {
  content: "";
  background-color: #ffffff !important;
  color: #ffffff;
  position: absolute;
  right: 0;
  top: 0.5rem;
  width: 28px;
  height: 3px;
}
.myBrowseBtn-toggler::before {
  content: "";
  position: absolute;
  top: -8px;
  width: 28px;
  height: 3px;
  background-color: #ffffff !important;
  color: #ffffff;
}
.myBrowseBtn-toggler::after {
  content: "";
  position: absolute;
  top: 8px;
  width: 20px;
  height: 3px;
  background-color: #ffffff !important;
  color: #ffffff;
} */
</style>