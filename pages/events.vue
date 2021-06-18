<template>
  <div>
    <eventsHero />
    <pastEvents />
    <upcomingEvents />
    <hostWebinar />
  </div>
</template>
<script>
  import eventsHero from "@/components/Events/heroSection.vue" 
  import pastEvents from "@/components/Events/pastEvents.vue";
  import upcomingEvents from "@/components/Events/upcomingEvents.vue";
  import hostWebinar from '@/components/Events/hostWebinar.vue';
  export default {
    components: {
      eventsHero,
      pastEvents,
      upcomingEvents,
      hostWebinar
    }
  }

</script>
<style scoped>

</style>
