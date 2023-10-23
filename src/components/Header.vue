<script>
import script from '../data/script';
export default {
  name: 'Header',

  data () {
    return {
      script
    }
  }
}
</script>

<template>
  <header>
    <div class="container">
      <!-- orari d'ufficio  -->
      <div class="hours">
        <p><i class="fa-solid fa-clock"></i> Open Hours: Mon - Sat - 9:00 - 18:00</p>
      </div>

      <!-- i contatti e social  -->
      <div class="contacts">
        <ul>
          <li v-for="(item, index) in script.headerContactsList" :key="index" ><a :href="item.href"><i :class="item.icon"></i></a>
             <a :href="item.href">  {{ item.content }}</a></li>
    
        </ul>
      </div>

    </div>

  </header>
</template>

<style lang="scss" scoped>
@use "../scss/partials/variables" as *;
@use "../scss/main.scss" as *;

header {
  height: 50px;
  background-color: $bg-header;
    .container {
      display: flex;
      justify-content: space-between;
      color: $grey-text;
      .hours {
      height: $h-100;
      text-align: start;
      line-height: 50px;
      }
      .contacts {
      height: $h-100;
      text-align: end;
      line-height: 50px;
        li {
          display: inline-block;
          margin-left: 25px;
            a {
              color: $grey-text;
              margin-left: 7px;
                &:hover {
                  text-decoration: underline;
                }
            }
        }
      } 
    }
   
}

</style>