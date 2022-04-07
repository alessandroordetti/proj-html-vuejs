<template>
  <div id="app">
    <IndexHeader />

    <IndexJumbotron class="section"/>

  </div>
</template>

<script>
import IndexHeader from './components/IndexHeader.vue';
import IndexJumbotron from './components/IndexJumbotron.vue';



export default {
  name: 'App',
  components: {
    IndexHeader,
    IndexJumbotron,
    
  }
}
</script>

<style lang="scss">
@import '@/style/main-style.scss';


</style>
