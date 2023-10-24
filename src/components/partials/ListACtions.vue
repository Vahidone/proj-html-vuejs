
<script>
export default {
  name: 'ListActions',

  data () {
    return {
      ListActions: [
        {
          content: "ALL"
        },
        {
          content: "INSTITUTIONAL"
        },
        {
          content: "SOCIAL"
        },
        {
          content: "EVENTS"
        },
        {
          content: "RESULTS"
        },
        {
          content: "INNOVATION"
        },
        {
          content: "ENVIRONMENT"
        },
        {
          content: "TECHNOLOGY"
        }
      ],
      activeIndex: null,
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
    <li v-for="(list, index) in ListActions" :key="index" :class="{active : activeIndex === index}" ><a href="##" @click="setActive(index)">{{ list.content }}</a></li>
  </ul>
</template>


<style lang="scss" scoped>
@use "../../scss/main.scss" as *;
@use "../../scss/partials/variables" as *;

ul {
  li {
    margin-top: 70px;
    display: inline-block;
    margin-right: 20px;

    &.active a {
      color: $btn-green;
        background-color: #D9EBED;
        padding: 7px;
    }
    a {
      color: gray;
      &:hover {
        color: $btn-green;
        background-color: #D9EBED;
        padding: 7px;
        cursor: pointer;
      }
        
    }
      
  }

}


</style>