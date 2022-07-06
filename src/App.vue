<template>
  <div id="app">
    <PageHeader />

    <main>
      <MainContentSection />
    </main>
  </div>
</template>

<script>
// import MainContentSection from './components/MainContentSection.vue'
import PageHeader from './components/PageHeader.vue'
import MainContentSection from './components/MainContentSection.vue'

export default {
  name: 'App',
  components: {
    PageHeader,
    MainContentSection
    // HelloWorld
  }
}
</script>

<style lang="scss">
@import "./style/common.scss";
</style>
