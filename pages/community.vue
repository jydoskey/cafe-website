<template>
  <div>
    <heroSection />
    <communities />
  </div>
</template>
<script>
  import heroSection from "@/components/Community/heroSection.vue"
  import communities from "@/components/Community/ourCommunities.vue";
  export default {
    components: {
      heroSection,
      communities
    }
  }

</script>
<style scoped>

</style>
