<script>
import NewPlace from './NewPlace.vue';
import SectionMagazine from './SectionMagazine.vue'
export default {
  name: 'AppMain',
  components: {
    NewPlace,
    SectionMagazine
  }

}
</script>

<template>
  <main>
    <NewPlace />
    <SectionMagazine />
  </main>
</template>



<style lang="scss" scoped></style>