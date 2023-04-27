<script>
import NewPlace from './NewPlace.vue';
import SectionMagazine from './SectionMagazine.vue'
import SectionPrice from './SectionPrice.vue';
import SectionBackground from './SectionBackground.vue'

export default {
  name: 'AppMain',
  components: {
    NewPlace,
    SectionMagazine,
    SectionPrice,
    SectionBackground
  }

}
</script>

<template>
  <main>
    <NewPlace />
    <SectionMagazine />
    <SectionPrice />
    <SectionBackground />
  </main>
</template>



<style lang="scss" scoped></style>