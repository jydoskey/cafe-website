<template>
  <div>
    <pastEvents />
    <upcomingEvents />
    <hostWebinar />
  </div>
</template>
<script>
  import pastEvents from "@/components/Events/pastEvents.vue";
  import upcomingEvents from "@/components/Events/upcomingEvents.vue";
  import hostWebinar from '@/components/Events/hostWebinar.vue';
  export default {
    components: {
      pastEvents,
      upcomingEvents,
      hostWebinar
    }
  }

</script>
<style scoped>

</style>
