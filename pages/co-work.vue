<template>
  <div>
    <subscription />
    <gallery />
  </div>
</template>
<script>
  import gallery from "@/components/CoWorking/gallery.vue";
  import subscription from '@/components/CoWorking/subscription.vue';
  export default {
    components: {
      gallery,
      subscription
    }
  }

</script>
<style scoped>

</style>
