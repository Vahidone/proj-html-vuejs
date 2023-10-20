

<script>
export default {
  name: 'Cards-company'
}
</script>

<template>
  <div class="container-csm mt-5">
    <div class="row">
      <div class="col-6">
        <div class="card">
          <h2><i class="fa-solid fa-lock"></i>  Security</h2>
          <p>Lorem ipsum dolor sit amet <br> consectetur adipisicing elit.</p>
        </div>
      </div>

      <div class="col-6">
        <div class="card">
          <h2><i class="fa-solid fa-lock"></i>  Security</h2>
          <p>Lorem ipsum dolor sit amet <br> consectetur adipisicing elit.</p>
        </div>
      </div>

      <div class="col-6">
        <div class="card">
          <h2><i class="fa-solid fa-lock"></i>  Security</h2>
          <p>Lorem ipsum dolor sit amet <br> consectetur adipisicing elit.</p>
        </div>
      </div>

      <div class="col-6">
        <div class="card">
          <h2><i class="fa-solid fa-lock"></i>  Security</h2>
          <p>Lorem ipsum dolor sit amet <br> consectetur adipisicing elit.</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../../scss/main.scss" as *;
@use "../../scss/partials/variables" as *;

.card {
  background-color: $bg-section-company;
  color: white;
  margin-top: 30px;
  
}


</style>