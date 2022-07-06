<template>
  <div id="app">
    <PageHeader />

    <main>
      <MainContentSection />
      <IconInfoSection />
    </main>
  </div>
</template>

<script>
// import IconInfoSection from './components/IconInfoSection.vue'
import PageHeader from './components/PageHeader.vue'
import MainContentSection from './components/MainContentSection.vue'
import IconInfoSection from './components/IconInfoSection.vue'

export default {
  name: 'App',
  components: {
    PageHeader,
    MainContentSection,
    IconInfoSection
    // HelloWorld
  }
}
</script>

<style lang="scss">
@import "./style/common.scss";
</style>
