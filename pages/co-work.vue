<template>
  <div>
    <subscription />
    <bookSpace />
    <gallery />
  </div>
</template>
<script>
  import subscription from '@/components/CoWorking/subscription.vue';
  import bookSpace from "@/components/CoWorking/bookSpace.vue";
  import gallery from "@/components/CoWorking/gallery.vue";
  export default {
    components: {
      subscription,
      bookSpace,
      gallery
    }
  }

</script>
<style scoped>

</style>
