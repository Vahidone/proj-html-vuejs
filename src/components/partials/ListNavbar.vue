
<script>
export default {
  name: 'ListGeneric',

  data () {
    return {
      listNavbar: [
        {
          content: "HOME",
          href: "#"
        },
        {
          content: "SERVICES",
          href: "#"
        },
        {
          content: "ABOUT",
          href: "#"
        },
        {
          content: "PROJECTS",
          href: "#"
        },
        {
          content: "RESULTS",
          href: "#"
        },
        {
          content: "GET IN TOUCH",
          href: "#"
        }
      ]
    }
  }

}
</script>

<template>
  <ul>
    <li v-for="(list, index) in listNavbar" :key="index"><a :href="list.href">{{ list.content }}</a></li>
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