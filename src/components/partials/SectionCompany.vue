

<script>
import store from '../../data/store';
import CardsCompany from './Cards-company.vue';
export default {
  name: 'SectionCompany',
  data () {
    store
  },
  components: {
    CardsCompany
  }
}
</script>

<template>
  <section>
    <div class="about">
      <h6>ABOUT THE NETWORK</h6>
      <h1 class="me-3">The</h1>
      <h1>Company</h1>
      <p>For 12 years we have beel providing audit and warranty, financial <br>
      advice, risk advice, taxes and related services to select clients. </p>

      <CardsCompany />

      <button class="btn_green">GET IN TOUCH</button>
      <button class="btn_white">READ ME</button>

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
      padding: 120px 0px 120px 390px;
      color: white;

        h6 {
          color: #06A5A6;
          margin-bottom: 20px;
        }
        h1 {
          display: inline-block;
          font-weight: bold;
          background-color: #0E262D;
          padding: 10px;
        }
        h1:nth-child(3) {
          background-color: $bg-section-company;
        }

        p {
          color: rgb(189, 188, 188);
        }

        .btn_white {
          background-color: $bg-section-company;
          color: white;
          margin-top: 100px;
            &:hover {
              scale: 1.05;
              cursor: pointer;
            }
        }
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