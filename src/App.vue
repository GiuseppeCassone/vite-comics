<script>
  import AppHeader from './components/AppHeader.vue';
  import AppContent from './components/AppContent.vue';
  import AppMerchandise from './components/AppMerchandise.vue';
  import AppFooter from './components/AppFooter.vue';

   export default {
    components: {
      AppHeader,
      AppContent,
      AppMerchandise,
      AppFooter,
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
  <AppFooter></AppFooter>
  
</template>

<style lang="scss">
@use './styles/main' as *;

</style>
