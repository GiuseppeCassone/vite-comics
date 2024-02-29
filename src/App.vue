<script>
  import AppHeader from './components/AppHeader.vue';
  import AppContent from './components/AppContent.vue';

   export default {
    components: {
      AppHeader,
      AppContent,
    },

    data(){
      return {
        
      }
    }
   }
</script>

<template>
  <AppHeader></AppHeader>
  <AppContent></AppContent>
</template>

<style lang="scss">
@use './styles/main' as *;

</style>
