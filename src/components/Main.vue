<script>
import SectionActions from './partials/SectionActions.vue';
import SectionCompany from './partials/SectionCompany.vue';
import SectionExcellence from './partials/SectionExcellence.vue';
import SectionReady from './partials/SectionReady.vue';
export default {
  name: 'Main',
  components: {
    SectionReady,
    SectionExcellence,
    SectionCompany,
    SectionActions
  
  }
}
</script>

<template>
  <main>
    <SectionReady />
    <SectionExcellence />
    <SectionCompany />
    <SectionActions />
  </main>
</template>

<style lang="scss">

</style>