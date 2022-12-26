<script setup>
  import TheHeader from './components/Header.vue'
  import Hero from './components/Hero.vue'
  import Overview from './components/Overview.vue'
  import Benefits from './components/Benefits.vue'
  import Depositions from './components/Depositions.vue'
  import Download from './components/Download.vue'
  import Help from './components/Help.vue'
  import TheFooter from './components/Footer.vue'
</script>

<template>
  <div>
    <TheHeader />
    <Hero />
    <Overview />
    <Benefits />
    <Depositions />
    <Download />
    <Help />
    <TheFooter />
  </div>
</template>

<style scoped lang="scss">
  div {
    position: relative;
    background-color: #f8f9ff;
  }
</style>
