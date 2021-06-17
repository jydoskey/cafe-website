<template>
  <div>
    <ourSpace />
    <subscription />
    <bookSpace />
    <gallery />
  </div>
</template>
<script>
  import ourSpace from "@/components/CoWorking/ourSpace.vue";
  import subscription from '@/components/CoWorking/subscription.vue';
  import bookSpace from "@/components/CoWorking/bookSpace.vue";
  import gallery from "@/components/CoWorking/gallery.vue";
  export default {
    components: {
      ourSpace,
      subscription,
      bookSpace,
      gallery
    }
  }

</script>
<style scoped>

</style>
