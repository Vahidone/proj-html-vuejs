
<script>
export default {
  name: 'ListGeneric',

  data () {
    return {
      ListNavbar: [
        {
          content: "HOME"
        },
        {
          content: "SERVICES"
        },
        {
          content: "ABOUT"
        },
        {
          content: "PROJECTS"
        },
        {
          content: "RESULTS"
        },
        {
          content: "GET IN TOUCH"
        }
      ]
    }
  }

}
</script>

<template>
  <ul>
    <li v-for="(list, index) in ListNavbar" :key="index"><a href="#">{{ list.content }}</a></li>
  </ul>
</template>


<style lang="scss" scoped>
@use "../../scss/main.scss" as *;
@use "../../scss/partials/variables" as *;

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


</style>