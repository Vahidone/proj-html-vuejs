<script>

import store from "../data/store";
export default {
  name: 'Footer',

  data () {
    return {
     store
    }
  }
}
</script>

<template>
  <footer>
    <div class="top">
      <div class="container">
        <div class="my-row">
          
          <div class="col m-3">
            <img src="../assets/svgs/svg-7.svg" alt="">

            <p>A Functional HTML Template <br>
            for Corporate & Buisiness</p>

            <p><i class="fa-solid fa-phone"></i> +1 (305) 1234-5678</p>
            <p><i class="fa-solid fa-envelope"></i> hello@example.com</p>
            <p><i class="fa-solid fa-location-dot"></i> Main Avenue, 987</p>

            <button class="btn_white">GET IN TOUCH</button>
          </div>
          <div class="col m-3">
            <h2 class="mt-4">About</h2>
           <ul>
            <li v-for="(item, index) in store.footerListaUno" :key="index"><i :class="item.icon"></i><a :href="item.href">{{ item.content }}</a></li>
           </ul>
          </div>
          <div class="col m-3">
            <h2 class="mt-4">Servises</h2>

            <ul>
            <li v-for="(item, index) in store.footerListaDue" :key="index"><i :class="item.icon"></i><a :href="item.href">{{ item.content }}</a></li>
           </ul>
          </div>
          <div class="col m-3">
            <h2 class="mt-4">Support</h2>
            <ul>
            <li v-for="(item, index) in store.footerListaTre" :key="index"><i :class="item.icon"></i><a :href="item.href">{{ item.content }}</a></li>
           </ul>
          </div>
          
        </div>

      </div>

    </div>

    <div class="down">
      <div class="container">
        <p>Enjoy the low price. We are tracking any intention of piracy</p>
        <p><i class="fa-regular fa-copyright"></i> 2020 NEXGEN is Proudly Powered by <span>Codings</span>.</p>
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
            text-align: start;
            padding: 10px;
            background-color: #191920;

            ul {
              li {
                margin-top: 20px;
                i {
                    margin-right: 10px;
                  }
                a {
                  color: gray;
                }
              }
            }
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