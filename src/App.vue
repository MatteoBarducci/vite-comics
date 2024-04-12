<script>
  import AppHeader from './components/AppHeader.vue';
  import AppMain from './components/AppMain.vue';
  import AppLowerSection from './components/AppLowerSection.vue';
  import AppFooter from './components/AppFooter.vue';
  import AppFooterBtm from './components/AppFooterBtm.vue';




  export default{
    components: {
      AppHeader,
      AppMain,
      AppLowerSection,
      AppFooter,
      AppFooterBtm,
    }
  }
</script>

<template>
  <AppHeader></AppHeader>
  <main>
    <AppMain></AppMain>
    <AppLowerSection></AppLowerSection>
  </main>
  <AppFooter></AppFooter>
  <AppFooterBtm></AppFooterBtm>
</template>

<style lang="scss">
  @use './style/generic.scss';
</style>
