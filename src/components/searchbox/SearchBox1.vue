<template>
  <div class="input-group mt-2 mb-2">
  <input type="text" class="form-control input-searchbox" aria-label="Text input with dropdown button" placeholder="Search products...">
  <div class="input-group-append">
    <!-- btn-outline-secondary -->
    <button class="btn  dropdown-toggle border-top border-bottom" type="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">Categories</button>
    <div class="dropdown-menu">
      <a class="dropdown-item" href="#">Categori x</a>
      <a class="dropdown-item" href="#">Categori x</a>
      <a class="dropdown-item" href="#">Categori x</a>
    </div>
    <button class="btn btn-search " type="button"><i class="fas fa-search"></i></button>
  </div>
</div>
</template>

<script>
export default {

}
</script>

<style scoped>
.btn-search {
  background-color: #20d3c2 !important;
  color: #FFFFFF;
  border-radius: 0 50% 50% 0;
  outline: none;
}

.input-searchbox {
  /* min-width: 250px; */
  border-radius: 50px 0 0 50px;
}
</style>