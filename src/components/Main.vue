<script>
import SectionTouch from './partials/Section-touch.vue'
import SectionResults from './partials/SectionResults.vue';
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
    SectionActions,
    SectionResults,
    SectionTouch
  
  }
}
</script>

<template>
  <main>
    <SectionReady />
    <SectionExcellence />
    <SectionCompany />
    <SectionActions />
    <SectionResults />
    <SectionTouch />
  </main>
</template>

<style lang="scss">

</style>