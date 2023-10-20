

<script>
export default {
  name: 'Navbar'
}
</script>

<template>
  <nav>
    <img src="../../assets/svgs/svg-7.svg" alt="">
    <div class="menu">
      <ul>
        <li><a href="#">HOME</a></li>
        <li><a href="#">SERVICES</a></li>
        <li><a href="#">ABOUT</a></li>
        <li><a href="#">PROJECTS</a></li>
        <li><a href="#">RESULTS</a></li>
        <li><a href="#">GET IN TOUCH</a></li>
      </ul>
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
       li {
        display: inline-block;
        margin-left: 25px;
         
          a {
            color: #3E4D57;
            &:hover {
            padding: 10px 5px;
            background-color: $btn-green;
            text-decoration: none;
            color: white;
          }
          }
       }
    }
}


</style>