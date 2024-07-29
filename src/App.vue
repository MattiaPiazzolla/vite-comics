<script>
// importo la componete per l'header
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppBanner from './components/AppBanner.vue';
export default {
  components: {
    AppHeader,
    AppMain,
    AppBanner
  }
}
</script>
<template>
  <div>
    <AppHeader />
    <AppMain />
    <AppBanner />
  </div>
</template>
<style lang="scss">
  @use './styles/generals.scss';

</style>