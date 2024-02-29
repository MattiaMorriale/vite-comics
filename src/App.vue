<script>

  import AppNav from './components/AppNav.vue';

  import AppMain from './components/AppMain.vue';

  import AppFooter from './components/AppFooter.vue';

  export default {

    components: {
      AppNav,
      AppMain,
      AppFooter,
    }

  }

  

</script>

<template>

<div class="container">
  <AppNav></AppNav>

  <AppMain></AppMain>

  <AppFooter></AppFooter>
</div>

</template>

<style>

</style>
