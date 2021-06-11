<template>
  <div>
    <aboutCafeone />
    <takeTour />
    <upcomingEvents />
    <cafeLocations />
  </div>
</template>
<script>
  import aboutCafeone from "@/components/Homepage/aboutCafe.vue";
  import takeTour from "@/components/Homepage/takeTour.vue";
  import upcomingEvents from "@/components/Homepage/upcomingEvents.vue";
  import cafeLocations from "@/components/Homepage/cafeLocations.vue";
  export default {
    components: {
      aboutCafeone,
      takeTour,
      upcomingEvents,
      cafeLocations
    }
  }

</script>
<style scoped>

</style>
