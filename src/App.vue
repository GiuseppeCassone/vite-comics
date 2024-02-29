<script>
  import AppHeader from './components/AppHeader.vue';
  import AppContent from './components/AppContent.vue';
  import AppMerchandise from './components/AppMerchandise.vue';

   export default {
    components: {
      AppHeader,
      AppContent,
      AppMerchandise,
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
  <AppMerchandise></AppMerchandise>
</template>

<style lang="scss">
@use './styles/main' as *;

</style>
