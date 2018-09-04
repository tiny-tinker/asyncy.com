<template>
  <div>
    <app-header/>
    <nuxt/>
    <app-footer/>
  </div>
</template>

<script>
  import AppHeader from '../components/Header/Header.vue';
  import AppFooter from '../components/Footer/Footer.vue';

  export default {
    components: {
      AppHeader,
      AppFooter
    }
  }
</script>

<style>
</style>

