<script>
  import AppHeader from './components/AppHeader.vue';
  import AppMain from './components/AppMain.vue';
  import AppLowerSection from './components/AppLowerSection.vue';


  export default{
    components: {
      AppHeader,
      AppMain,
      AppLowerSection,
    }
  }
</script>

<template>
  <AppHeader></AppHeader>
  <main>
    <AppMain></AppMain>
    <AppLowerSection></AppLowerSection>
  </main>
</template>

<style lang="scss">
  @use './style/generic.scss';
</style>
