<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppMerch from './components/AppMerch.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter,
    AppMerch
  }
}
</script>

<template>
  <AppHeader />

  <AppMain />

  <AppMerch />

  <AppFooter />
</template>

<style lang="scss">
@use './style/main.scss'
</style>
