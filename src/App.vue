<template>
  <div id="app">
    <PageHeader />
    <MainBanner />
    <main>
      <MainContentSection />
      <IconInfoSection />
    </main>

    <PageFooter />
  </div>
</template>

<script>
// import PageFooter from './components/PageFooter.vue'
import PageHeader from './components/PageHeader.vue'
import MainBanner from './components/MainBanner.vue'
import MainContentSection from './components/MainContentSection.vue'
import IconInfoSection from './components/IconInfoSection.vue'
import PageFooter from './components/PageFooter.vue'


export default {
  name: 'App',
  components: {
    PageHeader,
    MainBanner,
    MainContentSection,
    IconInfoSection,
    PageFooter
    // HelloWorld
  }
}
</script>

<style lang="scss">
@import "./style/common.scss";
</style>
