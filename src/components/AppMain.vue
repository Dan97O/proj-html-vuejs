<script>
import NewPlace from './NewPlace.vue';
import SectionMagazine from './SectionMagazine.vue'
import SectionPrice from './SectionPrice.vue';
export default {
  name: 'AppMain',
  components: {
    NewPlace,
    SectionMagazine,
    SectionPrice
  }

}
</script>

<template>
  <main>
    <NewPlace />
    <SectionMagazine />
    <SectionPrice />

  </main>
</template>



<style lang="scss" scoped></style>