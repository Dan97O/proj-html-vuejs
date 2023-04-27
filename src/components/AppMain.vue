<script>
import NewPlace from './NewPlace.vue';
import SectionMagazine from './SectionMagazine.vue';
import SectionPrice from './SectionPrice.vue';
import SectionBackground from './SectionBackground.vue';
import SectionTeams from './SectionTeams.vue';
import SectionBrand from './SectionBrand.vue'
import SectionFlavor from './SectionFlavor.vue'
import SectionPizza from './SectionPizza.vue'

export default {
  name: 'AppMain',
  components: {
    NewPlace,
    SectionMagazine,
    SectionPrice,
    SectionBackground,
    SectionTeams,
    SectionBrand,
    SectionFlavor,
    SectionPizza,
  }

}
</script>

<template>
  <main>
    <NewPlace />
    <SectionMagazine />
    <SectionPrice />
    <SectionBackground />
    <SectionTeams />
    <SectionBrand />
    <SectionFlavor />
    <SectionPizza />
  </main>
</template>



<style lang="scss" scoped></style>