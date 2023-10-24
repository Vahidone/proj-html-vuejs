

<script>
import store from '../../data/store'
export default {
  name: 'SectionResults',
  data() {
    return {
      store
    }
  }
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
          <div class="col-3" v-for="(item, index) in store.CrardArrResults" :key="index">
            <h1>{{item.number}}</h1>
            <span>{{item.name}}</span>
          </div>

        </div>

      </div>
    
      
    </div>


    <div class="down">
      <div class="container">
        <ul>
        <li v-for="(item, index) in store.logoArrResults" :key="index">
          <img :src="item.img">
        </li>
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
          font-size: 1.8rem;
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
            width: 90px;
            height: 30px;
          }
        }
      }

    }
     
    
  }
}


</style>