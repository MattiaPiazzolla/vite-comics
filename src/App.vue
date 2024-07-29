<script>
// importo la componete per l'header
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppBanner from './components/AppBanner.vue';
import AppFooter from './components/AppFooter.vue';
export default {
  components: {
    AppHeader,
    AppMain,
    AppBanner,
    AppFooter
  }
}
</script>
<template>
  <div>
    <AppHeader />
    <AppMain />
    <AppBanner />
    <AppFooter />
  </div>
</template>
<style lang="scss">
  @use './styles/generals.scss';

</style>