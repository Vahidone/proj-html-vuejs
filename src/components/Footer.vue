<script>
export default {
  name: 'Footer'
}
</script>

<template>
  <footer>
    <div class="top">
      <div class="container">
        <div class="my-row">
          
          <div class="col">
            <img src="../assets/svgs/svg-7.svg" alt="">

            <p>A Functional HTML Template <br>
            for Corporate & Buisiness</p>

            <p><i class="fa-solid fa-phone"></i> +1 (305) 1234-5678</p>
            <p><i class="fa-solid fa-envelope"></i> hello@example.com</p>
            <p><i class="fa-solid fa-location-dot"></i> Main Avenue, 987</p>

            <button class="btn_white">GET IN TOUCH</button>
          </div>
          <div class="col">
            <h2>About</h2>
            <ul>
              <li><i class="fa-solid fa-chevron-right"></i> vahid ban</li>
              <li><i class="fa-solid fa-chevron-right"></i> vahid ban</li>
              <li><i class="fa-solid fa-chevron-right"></i> vahid ban</li>
              <li><i class="fa-solid fa-chevron-right"></i> vahid ban</li>
              <li><i class="fa-solid fa-chevron-right"></i> vahid ban</li>
              <li><i class="fa-solid fa-chevron-right"></i> vahid ban</li>
            </ul>
          </div>
          <div class="col">
            <h2>Servises</h2>
            <ul>
              <li><i class="fa-solid fa-chevron-right"></i> vahid ban</li>
              <li><i class="fa-solid fa-chevron-right"></i> vahid ban</li>
              <li><i class="fa-solid fa-chevron-right"></i> vahid ban</li>
              <li><i class="fa-solid fa-chevron-right"></i> vahid ban</li>
              <li><i class="fa-solid fa-chevron-right"></i> vahid ban</li>
              <li><i class="fa-solid fa-chevron-right"></i> vahid ban</li>
            </ul>
          </div>
          <div class="col">
            <h2>Support</h2>
            <ul>
              <li><i class="fa-solid fa-chevron-right"></i> vahid ban</li>
              <li><i class="fa-solid fa-chevron-right"></i> vahid ban</li>
              <li><i class="fa-solid fa-chevron-right"></i> vahid ban</li>
              <li><i class="fa-solid fa-chevron-right"></i> vahid ban</li>
              <li><i class="fa-solid fa-chevron-right"></i> vahid ban</li>
              <li><i class="fa-solid fa-chevron-right"></i> vahid ban</li>
            </ul>
          </div>
          
        </div>

      </div>

    </div>

    <div class="down">
      <div class="container">
        <p>Enjoy the low price. We are tracking any intention of piracy</p>
        <p><i class="fa-regular fa-copyright"></i> 2020 NEXGEN is Proudly Powered by <span>Codings</span></p>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
@use "../scss/partials/variables" as *;
@use "../scss/main.scss" as *;
footer {
  .top {
    background-color: $bg-footer;
    height: 620px;
      .container {
        color: white;
        height: 100%;
        display: flex;
        justify-content: space-between;
        justify-content: center;
        align-items: center;
        .my-row {
          width: $w-100;
          display: flex;
          justify-content: space-between;
          color: gray;
          .col {
            width: 25%;
            height: $h-100;
            text-align: center;
            background-color: #191920;
            button {
              background-color: #111118;
            }
            h2 {
              margin-left: 40px;
              color: white;
            }
           
            p {
              margin-bottom: 20px;
             
            }
            p:nth-child(2) {
              margin-bottom: 30px;
            }
            ul {
              li {
                margin-top: 20px
              }
            }
           
    
          }

          .col:first-child {
            background-color: #111118;
            text-align: start;
            img {
              width: 140px;
              height: 50px;
              margin-bottom: 25px;
              margin-left: 0;
            }
          }
        } 
       
      }
  }
  .down {
    background-color: black;
    height: 80px;
      .container {
        display: flex;
        justify-content: space-between;
        line-height: 80px;
          p {
            color: gray;
              span {
                color: $btn-green;
              }
          }
      }
  }
}

</style>