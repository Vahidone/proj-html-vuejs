

<script>
import ListNavbar from './ListNavbar.vue';
export default {
  name: 'Navbar',
  components: {
    ListNavbar
  }
}
</script>

<template>
  <nav>
    <img src="../../assets/svgs/svg-7.svg" alt="">
    <div class="menu">
     <ListNavbar />
    </div>

  </nav>
 
</template>

<style lang="scss" scoped>
@use "../../scss/main.scss" as *;
@use "../../scss/partials/variables" as *;
nav {
  width: $w-100;
  height: 80px;
  display: flex;
  justify-content: space-between;
    img {
      width: 165px;
      height: 40px;
      margin: auto 0;
    }
    .menu {
      height: 100%;
      line-height: 80px;
    }
}


</style>