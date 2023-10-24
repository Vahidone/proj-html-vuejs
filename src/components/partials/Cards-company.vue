

<script>
import store from '../../data/store';
export default {
  name: 'CardsCompany',

  data () {
    return {
      store
    }
    
  },
 

}
</script>

<template>
 
  <div class="row">
    <div class="col-6" v-for="(card, index) in store.cardsArrCompany" :key="index">
      <div class="card" >
        <h4><i :class="card.icon"></i>  {{ card.title }}</h4>
        <p>{{ card.content}}</p>
      </div>
    </div>
  </div>

</template>

<style lang="scss" scoped>
@use "../../scss/main.scss" as *;
@use "../../scss/partials/variables" as *;

.row {

  .card {
    width: 100%;
    background-color: $bg-section-company;
    color: white;
    margin-top: 30px;
      p {
        color: rgb(189, 188, 188);
      }

      i {
        color: $btn-green;
      }
  
  }
}




</style>