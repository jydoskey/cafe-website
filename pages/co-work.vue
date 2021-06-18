<template>
  <div>
    <heroSection />
    <features />
    <ourSpace />
    <subscription />
    <bookSpace />
    <gallery />
  </div>
</template>
<script>
  import heroSection from "@/components/CoWorking/heroSection";
  import features from "@/components/CoWorking/features.vue";
  import ourSpace from "@/components/CoWorking/ourSpace.vue";
  import subscription from '@/components/CoWorking/subscription.vue';
  import bookSpace from "@/components/CoWorking/bookSpace.vue";
  import gallery from "@/components/CoWorking/gallery.vue";
  export default {
    components: {
      heroSection,
      features,
      ourSpace,
      subscription,
      bookSpace,
      gallery
    }
  }

</script>
<style scoped>

</style>
