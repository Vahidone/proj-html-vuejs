

<script>
export default {
  name: 'SectionResults'
}
</script>

<template>

  <section>
    <div class="top">
      <div class="container">
        <h6>WHAT ARE WE DOING</h6>
        <h1>Results</h1>
        <h1 class="ms-3">in Numbers</h1>
        <div class="row">
          <div class="col-3">
            <h1>128</h1>
            <span>Certifications</span>
          </div>

          <div class="col-3">
            <h1>128</h1>
            <span>Certifications</span>
          </div>

          <div class="col-3">
            <h1>128</h1>
            <span>Certifications</span>
          </div>

          <div class="col-3">
            <h1>128</h1>
            <span>Certifications</span>
          </div>
        </div>

      </div>
    
      
    </div>


    <div class="down">
      <div class="container">
        <ul>
        <li><img src="../../assets/img/logo-4.png" alt=""></li>
        <li><img src="../../assets/img/logo-5.png" alt=""></li>
        <li><img src="../../assets/img/logo-1.png" alt=""></li>
        <li><img src="../../assets/img/logo-2.png" alt=""></li>
        <li><img src="../../assets/img/logo-3.png" alt=""></li>
        <li><img src="../../assets/img/logo-4.png" alt=""></li>
      </ul>

      </div>
    
    </div>
  </section>


  
</template>

<style lang="scss" scoped>
@use "../../scss/main.scss" as *;
@use "../../scss/partials/variables" as *;

section {
  text-align: center;
  .top {
  height: 590px;
  padding: 130px 10px;
  background-image: url(../../assets/img/bg-7.jpg);
     h6 {
      color: $btn-green;
      margin-bottom: 20px;
    }

    h1 {
      display: inline-block;
      font-size: 3rem;
      font-weight: bold;
      color: white;
    }

    h1:nth-child(2) {
      background-color: #0C2B2C;
      padding: 5px 10px;
    }

    .row {
      margin-top: 80px;
      display: flex;
      justify-content: space-between;

        h1 {
          color: $btn-green;
          font-weight: bold;
        }
        span {
          color: white;
          font-size: 1.5rem;
          font-weight: bold;
          display: block;
        }
    }

 

  }

  .down {
    height: 280px;
    background-color: #111118;
    .container {
      height: $h-100;
      line-height: 280px;
      ul {
        display: flex;
        justify-content: space-between;
        li {
          img {
            width: 100px;
            height: 30px;
          }
        }
      }

    }
     
    
  }
}


</style>