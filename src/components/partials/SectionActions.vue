

<script>
import CardsActions from './Cards-actions.vue';
import ListACtions from './ListACtions.vue';
export default {
  name: 'SectionActions',
  components: {
    CardsActions,
    ListACtions
  }
}
</script>

<template>
  <section>
    <div class="container">
    <div class="top">
      <h6>WE DO MORE FOR EVERYONE</h6>
      <h1>Actions &</h1>
      <h1 class="h1-b">Projects</h1>

      <ListACtions />
    </div>

    <div class="down">
      <CardsActions />
    </div>
  </div>

  </section>

</template>

<style lang="scss" scoped>
@use "../../scss/main.scss" as *;
@use "../../scss/partials/variables" as *;
section {
  height: 1300px;
  padding-top: 130px;
  .top {
    text-align: center;
    
    h6 {
      color: #06A5A6;
      margin-bottom: 20px;
    }
   
    h1 {
      display: inline-block;
      font-weight: bold;
      font-size: 3rem;
      margin-right: 20px
    }

    .h1-b {
      color: $btn-green;
      background-color: #D9EBED;
      padding: 5px 10px;
    }
  }
}


</style>