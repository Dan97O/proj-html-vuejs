<script>
import SectionFooter from './SectionFooter.vue'
export default {
  name: 'AppFooter',

  components: {
    SectionFooter
  },
  data() {
    return {
      restaurants: [
        {
          address: "1614 E. Bell Rd #104",
          city: "Salerno, AZ 85022",
          phone: "(602) 867-1010"
        },
        {
          address: "204 E. Pizzetta Tommaso",
          city: "Sorrento, AZ 85022",
          phone: "(358) 867-1010"
        },
        {
          address: "Vale Puglia 54",
          city: "Torre del Greco, AZ 85022",
          phone: "(359) 867-1010"
        },
        {
          address: "Corso Itali AA",
          city: "Naples, AZ 85022",
          phone: "(989) 867-1010"
        }
      ],
      working: [
        {
          day: "MONDAY",
          time: "Kitchen Closed",
        },
        {
          day: "TUSEDAY UNTIL FRIDAY",
          time: "9:00 - 22:00",
        },
        {
          day: "SATURDAY*",
          time: "Saturday 11am to midnigth",
        },
        {
          day: "SUNDAY",
          time: "9:00 - 22:00",
        }
      ]
    };
  },
}
</script>


<template>
  <footer>
    <SectionFooter :restaurants="restaurants" :working="working" />
  </footer>
</template>


<style lang="scss">
footer {
  font-family: "Poppins";
  font-size: 16px;
}
</style>