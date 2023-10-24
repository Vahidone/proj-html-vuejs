

<script>
import store from '../../data/store'
export default {
  name: 'Cards-actions',
  data () {
    return {
      store
    }
  }

}
</script>

<template>
  <div class="container">
    <div class="row">
      <div class="col-4" v-for="(card, index) in store.cardsArrAction" :key="index">
        <div class="card relative">
          <img :src="card.img" alt="">
          <h3>{{card.title}}</h3>
          <div class="filter"></div>
        </div> 
      </div>
      
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../../scss/main.scss" as *;
@use "../../scss/partials/variables" as *;

.row {
  flex-direction: row;
  flex-wrap: wrap;
  .card {
  width: 100%;
  height: 350px;
  margin-top: 25px;
  text-align: center;
  border-radius: 10px;
  overflow: hidden;
   &:hover {
    scale: 1.05;
    transition: all 1s;
    cursor: pointer;
   }
  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }

  .filter {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, .3)
  }
  h3 {
    position: absolute;
    bottom: 40px;
    left: 50px;
    color: white;
  }
  
}

}








</style>