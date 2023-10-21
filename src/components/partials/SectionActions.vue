

<script>
import CardsContainerActions from './CardsContainer-actions.vue';
export default {
  name: 'SectionActions',
  components: {
    CardsContainerActions
  }
}
</script>

<template>
  <section>
    <div class="container">
    <div class="top">
      <h5>WE DO MORE FOR EVERYONE</h5>
      <h1>Actions &</h1>
      <h1>Projects</h1>

      <ul>
        <li><a href="">ALL</a> </li>
        <li><a href="">INSTITUTIONAL</a> </li>
        <li><a href="">SOCIAL</a></li>
        <li><a href="">EVENTS</a></li>
        <li><a href="">INNOVATION</a></li>
        <li><a href="">ENVIRONMENT</a></li>
        <li><a href="">TECHNOLOGY</a></li>
      </ul>
    </div>

    <div class="down">
      <CardsContainerActions />
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
    li {
      display: inline-block;
      margin-right: 20px;
        a {
          color: gray;
        }
    }
    h1 {
      display: inline-block;
      font-weight: bold;
      font-size: 3rem;
    }
}
}


</style>