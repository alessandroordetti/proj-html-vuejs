<template>
  <div id="app">
    <IndexHeader />

    <IndexMain />

    <IndexFooter />
  </div>
</template>

<script>
import IndexHeader from './components/IndexHeader.vue';
import IndexMain from './components/IndexMain.vue';
import IndexFooter from './components/IndexFooter.vue'



export default {
  name: 'App',
  components: {
    IndexHeader,
    IndexMain,
    IndexFooter,
  }
}
</script>

<style lang="scss">
@import '@/style/main-style.scss';


</style>
