

<script>
export default {
  name: 'SectionCompany'
}
</script>

<template>
  <section>
    <div class="about">
      <h6>ABOUT THE NETWORK</h6>
      <h1>The</h1>
      <h1>Company</h1>
      <p>For 12 years we have beel providing audit and warranty, financial <br>
      advice, risk advice, taxes and related services to select clients. </p>
      
    </div>

    <figure class="debbug">
      <img src="../../assets/img/about-4.jpg" alt="">
    </figure>
  </section>
</template>

<style lang="scss" scoped>
@use "../../scss/main.scss" as *;
@use "../../scss/partials/variables" as *;
section {
  height: 880px;
  background-color: $bg-section-company;
  display: flex;
    .about {
      width: 50%;
      height: $h-100;
      padding-left: 390px;
    }
    figure {
      width: 50%;
      height: $h-100;
       img {
        width: $w-100;
        height: $h-100;
        object-fit: cover;
       }
    }
}

</style>