<script>
import SectionCompany from './partials/SectionCompany.vue';
import SectionExcellence from './partials/SectionExcellence.vue';
import SectionReady from './partials/SectionReady.vue';
export default {
  name: 'Main',
  components: {
    SectionReady,
    SectionExcellence,
    SectionCompany
  
  }
}
</script>

<template>
  <main>
    <SectionReady />
    <SectionExcellence />
    <SectionCompany />
  </main>
</template>

<style lang="scss">

</style>