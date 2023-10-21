

<script>
export default {
  name: 'Cards-actions'

}
</script>

<template>
  <div class="container">
    <div class="row">
      <div class="col-4">
        <div class="card relative">
          
          <div class="filter">sono filter</div>
          <h3>Academic Professional <br>program in social media</h3>
        </div> 
      </div>
      <div class="col-4">
        <div class="card relative">
          <h3>Academic Professional <br>program in social media</h3>
          <div class="filter">sono filter</div>
        </div>
        
      </div>
      <div class="col-4">
        <div class="card relative">
          <h3>Academic Professional <br>program in social media</h3>
          <div class="filter">sono filter</div>
        </div>
        
      </div>
      <div class="col-4">
        <div class="card relative">
          <h3>Academic Professional <br>program in social media</h3>
          <div class="filter">sono filter</div>
        </div>
        
      </div>
      <div class="col-4">
        <div class="card relative">
          <h3>Academic Professional <br>program in social media</h3>
          <div class="filter">sono filter</div>
        </div>
        
      </div>
      <div class="col-4">
        <div class="card relative">
          <h3>Academic Professional <br>program in social media</h3>
          <div class="filter">sono filter</div>
        </div>
        
      </div>

      
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../../scss/main.scss" as *;
@use "../../scss/partials/variables" as *;


.card {
  
  height: 350px;
  margin-top: 25px;
  background-image: url(../../assets/img/project-1.jpg);
  text-align: center;
  padding-top: 260px;
  .filter {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, .3)
  }
  h3 {
    color: white;
  }
  
}







</style>