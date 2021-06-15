<template>
  <div>
    <bookSpace />
    <subscription />
    <gallery />
  </div>
</template>
<script>
  import bookSpace from "@/components/CoWorking/bookSpace.vue";
  import subscription from '@/components/CoWorking/subscription.vue';
  import gallery from "@/components/CoWorking/gallery.vue";
  export default {
    components: {
      bookSpace,
      subscription,
      gallery
    }
  }

</script>
<style scoped>

</style>
