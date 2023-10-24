
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
      ],
      activeIndex: null
    }
  },

  methods: {
    setActive(index) {
      this.activeIndex = index;
    }
  }
}
</script>




<template>
  <ul>
    <li v-for="(list, index) in listNavbar" :key="index" :class="{ active: activeIndex === index }">
      <a :href="list.href" @click="setActive(index)">{{ list.content }}</a>
    </li>
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
    padding: 10px 5px;
    text-decoration: none;
    
  }

  &.active a, a:hover {
    background-color: $btn-green;
    color: white;
  }

 
}
</style>
