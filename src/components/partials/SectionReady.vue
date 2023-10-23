

<script>
import Navbar from './Navbar.vue';
export default {
  name: 'SectionReady',
  components: {
    Navbar,
   
  }
}
</script>

<template>
  <div class="bg">
  
    <section>
      <div class="container">
        <Navbar />
        <div class="box-raed-me">
          <div class="read-me">
            <h1 class="h1">Ready</h1>
            <h1 class="h1-b">Team</h1>
            <p>No matter what your company needs, we will be <br>
            ready to assist you in the best possibile way.</p>

            <button class="btn_green">GET IN TOUCH</button>
            <button class="btn_white">READ ME</button>
          </div>
        </div>
      </div>
    </section>

    <div class="right-side">
      <div></div>
      <div></div>
      <div></div>
    </div>
  </div>
 
 
</template>

<style lang="scss" scoped>
@use "../../scss/main.scss" as *;
@use "../../scss/partials/variables" as *;
.bg {
  height: 860px;
  background-color: white;
  display: flex;
  .right-side {
    width: 60px;
    height: $h-100;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
     
      div {
        width: 12px;
        height: 35px;
        border-radius: 40px;
        border: 2px solid #068283;
        margin-top: 10px;
          &:nth-child(2) {
          background-color: #068283;
          }
        
      }
  }
  section {
  width: calc(100% - 60px);
  height: $h-100;
  background-image: url(../../assets/img/bg-parallax.png);
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  display: flex;
  justify-content: center;
  align-items: center;
    .container {
      height: $h-100;
      .box-raed-me {
      width: $w-100;
      height: calc(100% - 80px);
      display: flex;
      justify-content: center;
      align-items: center;
      .read-me {
      width: 550px;
      height: 350px;
      text-align: center;
      padding: 20px;
        .h1 {
          font-size: 5.3rem;
          font-weight: bold;
          display: inline-block;

        }
        .h1-b {
          font-size: 5.3rem;
          font-weight: bold;
          display: inline-block;
          margin-left: 15px;
          color: #068283;
          padding: 5px 10px;
          background-color: #d2e1e1;
        }
        p {
          font-size: 20px;
          color: #aeb1bc;
        }

        .btn_white {
          background-color: white;
        }
       }
    }

    }
   
   
  }
}

</style>