<template>
  <div>
    <pastEvents />
    <upcomingEvents />
  </div>
</template>
<script>
  import pastEvents from "@/components/Events/pastEvents.vue";
  import upcomingEvents from "@/components/Events/upcomingEvents.vue"
  export default {
    components: {
      pastEvents,
      upcomingEvents
    }
  }

</script>
<style scoped>

</style>
