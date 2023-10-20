
<script>
export default {
  name: 'SectionExcellence'
}
</script>

<template>
  <section>
    <div class="container">
      <div class="top">
        <h6>OUR BUISINESS AREAS</h6>
        <h1 class="h1">Excellence in </h1>
        <h1 class="h1-b">Servises</h1>
        <p>We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of <br>
        experienced and renowned professionals. These are some options that you can hire.</p>

        <button class="btn_green">SEE ALL</button>
      </div>

      <div class="container">
        <div class="row d-flex">
          <div class="col-sm-4 mt-4">
            <div class="card py-5 px-3 bg-white">
              <div class="card-body">
                <div class="d-flex space-betw align-items-center ">
                  <img src="../../assets/svgs/svg-1.svg" alt="">
                  <span><i class="fa-solid fa-arrow-right"></i></span>
                </div>
                <h3 class="mt-4 fw-bold">Audit & Assurance</h3>
                <p class="mt-4"> Lorem ipsum dolor sit amet. <br>
                consectetor adipiscing elit.</p>
              </div>
            </div>
          </div>

          <div class="col-sm-4 mt-4">
            <div class="card py-5 px-3 bg-white">
              <div class="card-body">
                <div class="d-flex space-betw align-items-center ">
                  <img src="../../assets/svgs/svg-1.svg" alt="">
                  <span><i class="fa-solid fa-arrow-right"></i></span>
                </div>
                <h3 class="mt-4 fw-bold">Audit & Assurance</h3>
                <p class="mt-4"> Lorem ipsum dolor sit amet. <br>
                consectetor adipiscing elit.</p>
              </div>
            </div>
          </div>

          <div class="col-sm-4 mt-4">
            <div class="card py-5 px-3 bg-white">
              <div class="card-body">
                <div class="d-flex space-betw align-items-center ">
                  <img src="../../assets/svgs/svg-1.svg" alt="">
                  <span><i class="fa-solid fa-arrow-right"></i></span>
                </div>
                <h3 class="mt-4 fw-bold">Audit & Assurance</h3>
                <p class="mt-4"> Lorem ipsum dolor sit amet. <br>
                consectetor adipiscing elit.</p>
              </div>
            </div>
          </div>

          <div class="col-sm-4 mt-4">
            <div class="card py-5 px-3 bg-white">
              <div class="card-body">
                <div class="d-flex space-betw align-items-center ">
                  <img src="../../assets/svgs/svg-1.svg" alt="">
                  <span><i class="fa-solid fa-arrow-right"></i></span>
                </div>
                <h3 class="mt-4 fw-bold">Audit & Assurance</h3>
                <p class="mt-4"> Lorem ipsum dolor sit amet. <br>
                consectetor adipiscing elit.</p>
              </div>
            </div>
          </div>

          <div class="col-sm-4 mt-4">
            <div class="card py-5 px-3 bg-white">
              <div class="card-body">
                <div class="d-flex space-betw align-items-center ">
                  <img src="../../assets/svgs/svg-1.svg" alt="">
                  <span><i class="fa-solid fa-arrow-right"></i></span>
                </div>
                <h3 class="mt-4 fw-bold">Audit & Assurance</h3>
                <p class="mt-4"> Lorem ipsum dolor sit amet. <br>
                consectetor adipiscing elit.</p>
              </div>
            </div>
          </div>

          <div class="col-sm-4 mt-4">
            <div class="card py-5 px-3 bg-white">
              <div class="card-body">
                <div class="d-flex space-betw align-items-center ">
                  <img src="../../assets/svgs/svg-1.svg" alt="">
                  <span><i class="fa-solid fa-arrow-right"></i></span>
                </div>
                <h3 class="mt-4 fw-bold">Audit & Assurance</h3>
                <p class="mt-4"> Lorem ipsum dolor sit amet. <br>
                consectetor adipiscing elit.</p>
              </div>
            </div>
          </div>
    
        </div>

      </div>

    </div>
  </section>
</template>


<style lang="scss" scoped>
@use "../../scss/main.scss" as *;
@use "../../scss/partials/variables" as *;
section {
  height: 1100px;
  background-color: $bg-section-excellence;
    .container {
      padding: 100px 0;
       .top {

         h6 {
          color: #068283;
         }
         .h1 {
          font-size: 3.5rem;
          font-weight: bold;
          display: inline-block;

          }
          .h1-b {
          font-size: 3.5rem;
          font-weight: bold;
          display: inline-block;
          margin-left: 15px;
          color: #068283;
          padding: 5px 10px;
          background-color: #d2e1e1;
          }
          p {
            display: inline-block;
          }
          button {
            margin-left: 478px;
          }

        }
      .card-body {
        img {
          width: 40px;
          height: 40px;
          
        }
        span {
          font-size: 22px;
        }
      } 
    }
}

</style>