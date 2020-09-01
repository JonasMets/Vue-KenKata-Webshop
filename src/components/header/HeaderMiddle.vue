<template>
  <div class="container">
    <nav class="navbar navbar-expand-lg navbar-light">
      <Logo1></Logo1>
      <button
        class="navbar-toggler ml-auto"
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
        <ul class="navbar-nav">
          <li class="nav-item">
            <!-- <Logo1></Logo1> -->
          </li>
        </ul>

        <ul class="navbar-nav ml-auto">
          <li class="nav-item active border-right">
            <!-- serachbox -->
            <SearchBox1></SearchBox1>
          </li>

          <!--  -->
          <div>
            <ul class="navbar-nav ml-auto">
              <li class="nav-item">
                <MyAccount1></MyAccount1>
              </li>
              <!--  -->
            </ul>
          </div>
        </ul>
      </div>
    </nav>
  </div>
</template>

<script>
import Logo1 from "@/components/logo/Logo1";
import SearchBox1 from "@/components/searchbox/SearchBox1";
import MyAccount1 from "@/components/myaccount/MyAccount1";

export default {
  components: {
    //
    Logo1,
    SearchBox1,
    MyAccount1
  }
};
</script>

<style>
</style>