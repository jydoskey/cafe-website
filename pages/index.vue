<template>
  <div>
    <aboutCafeone />
    <takeTour />
    <cafeLocations />
  </div>
</template>
<script>
  import aboutCafeone from "@/components/Homepage/aboutCafe.vue";
  import takeTour from "@/components/Homepage/takeTour.vue";
  import cafeLocations from "@/components/Homepage/cafeLocations.vue";
  export default {
    components: {
      aboutCafeone,
      takeTour,
      cafeLocations
    }
  }

</script>
<style scoped>

</style>
