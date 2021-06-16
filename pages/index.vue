<template>
  <div>
    <homeHero />
    <aboutCafeone />
    <takeTour />
    <upcomingEvents />
    <cafeLocations />
  </div>
</template>
<script>
  import homeHero from "@/components/Homepage/heroSection.vue" 
  import aboutCafeone from "@/components/Homepage/aboutCafe.vue";
  import takeTour from "@/components/Homepage/takeTour.vue";
  import upcomingEvents from "@/components/Homepage/upcomingEvents.vue";
  import cafeLocations from "@/components/Homepage/cafeLocations.vue";
  export default {
    components: {
      homeHero,
      aboutCafeone,
      takeTour,
      upcomingEvents,
      cafeLocations
    }
  }

</script>
<style scoped>

</style>
