<template>
  <div class="d-flex justify-content-center align-items-center">
    <!-- <i class="far fa-user"></i> -->
    <a href="#" class="nav-link">
      <img src="@/assets/Usericon.png" alt /> My account
    </a>
    <!-- <i class="far fa-heart"></i> -->
    <a href="#" class="nav-link">
      <img src="@/assets/Hearticon.png" alt />
    </a>

    <div class="position-relative">
      <a href="#" class="nav-link">
        <img src="@/assets/Compareicon.png" alt />
      </a>
      <div class="badge badge-pill badge-primary myBadge1">0</div>
    </div>

    <!-- <a href="#" class="nav-link">
      <img src="@/assets/Bagicon.png" alt />
    </a> -->

    <div class="position-relative">
      <a href="#" class="nav-link">
        <img src="@/assets/Bagicon.png" alt />
      </a>
      <div class="badge badge-pill badge-primary myBadge1">0</div>
    </div>

    <span>$ 0.00</span>
    
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.myBadge1 {
  position: absolute;
  top: 1px;
  left: 17px;
  z-index: 2;
  background-color: #20d3c2 !important;
}
</style>