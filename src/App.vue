<template>
  <div id="app">
    <InputWithSeparator />
  </div>
</template>

<script>
  import InputWithSeparator from './components/InputWithSeparator.vue'

  export default {
    name: 'App',
    components: {
      InputWithSeparator
    }
  }
</script>

<style>
  #app {
    margin: 60px;
  }
</style>
