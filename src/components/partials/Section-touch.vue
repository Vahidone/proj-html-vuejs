
<script>
export default {
  name: 'SectionTouch'

}
</script>

<template>
  <section>
    <div class="container">
      <div class="left">
        <h6>SEND A MESSAGE</h6>

        <h1>Get in</h1>
        <h1 class="h1-b">Touch</h1>

        <p>We will respond to your messsage as soon as possible</p>

        <div class="my-form">
          <div class="row">
            <div class="col-6">
              <div class="mb-3">
                <input type="text" class="form-control" id="exampleFormControlInput1" placeholder="Name">
              </div>
            </div>

            <div class="col-6">
              <div class="mb-3">
                <input type="email" class="form-control" id="exampleFormControlInput1" placeholder="Email">
              </div>
            </div>

            <div class="col-6">
              <div class="mb-3">
                <input type="text" class="form-control" id="exampleFormControlInput1" placeholder="Phone">
              </div>
            </div>

            <div class="col-6">
              <select class="form-select" aria-label="Default select example">
                <option selected>More Info</option>
                <option value="1">One</option>
                <option value="2">Two</option>
                <option value="3">Three</option>
              </select>
            </div>
          </div>
        </div>


        <div class="mb-3">
          <textarea class="form-control" id="exampleFormControlTextarea1" rows="3" placeholder="Message"></textarea>
        </div>

        <button class="btn_green">SEND</button>
      </div>

      <div class="right">
        <h4 class="fw-bold">Example Inc.</h4>
        <p>Lorem ipsum dolor sit amet, consectetur <br> adipisicing elit.</p>

        <p>Praesenr diam lacus, dapibus sed imperdiet <br>consectetur</p>

        <ul>
          <li><a href="#"><i class="fa-solid fa-phone"></i> +1 (305) 1234-5678</a></li>
          <li><a href="#"><i class="fa-solid fa-envelope"></i> hello@example.com</a></li>
          <li><a href="#"><i class="fa-solid fa-location-dot"></i> Main Avenue, 987</a></li>
        </ul>

        <button class="btn_white bg-white">VIEW MAP</button>
      </div>
    </div>

  </section>
  
</template>


<style lang="scss" scoped>
@use "../../scss/main.scss" as *;
@use "../../scss/partials/variables" as *;
section {
  height: 850px;
  background-color: white;
    .container {
      display: flex;
      height: $h-100;
      .left {
        width: 70%;
        height: $h-100;
        padding: 100px 0;
        h6 {
          color: #068283;
        }
        h1 {
          font-weight: bold;
          display: inline-block;
        }
        
        .h1-b {
          color: #068283;
          margin-left: 10px;
          font-size: 3rem;
        }
        p {
          color: gray;
        }
        .my-form {
          div {
            input {
              background-color: #ECECEC;
            }
            select {
              background-color: #ECECEC;
              color: gray;
            }
          }
        }

        textarea {
          background-color: #ECECEC;
        }

          
      }
      .right {
        width: 30%;
        height: $h-100;
        padding: 100px 20px;
          li {
            a {
              color: #068283;
            }
          }
      }

    }
 
}


</style>