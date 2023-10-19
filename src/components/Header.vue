<script>
export default {
  name: 'Header'
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
          <li><a href="#"><i class="fa-solid fa-phone"></i>  +1 (305) 1234-5678</a></li>
          <li><a href="#"><i class="fa-solid fa-envelope"></i>  hello@example.com</a></li>
          <li><a href="#"><i class="fa-brands fa-facebook-f"></i></a></li>
          <li><a href="#"><i class="fa-brands fa-twitter"></i></a></li>
          <li><a href="#"><i class="fa-brands fa-linkedin-in"></i></a></li>
        </ul>
      </div>

    </div>

  </header>
</template>

<style lang="scss" scoped>
@use "../scss/partials/variables" as *;
@use "../scss/main.scss" as *;

header {
  height: 60px;
  background-color: $bg-header;
    .container {
      display: flex;
      justify-content: space-between;
      color: $grey-text;
      .hours {
      height: $h-100;
      text-align: start;
      line-height: 60px;
      }
      .contacts {
      height: $h-100;
      text-align: end;
      line-height: 60px;
        li {
          display: inline-block;
          margin-left: 25px;
            a {
              color: $grey-text;
            }
        }
      } 
    }
   
}

</style>