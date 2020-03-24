<template>
  <label>
    <input type="text" v-on:input="addSeparator" v-bind:value="viewerValue" />
  </label>
</template>

<script>
  export default {
    name: 'InputWithSeparator',
    data: function () {
      return {
        inputValue: ''
      };
    },
    computed: {
      viewerValue: function () {
        const cleanValue = this.inputValue.replace(/-/g, '');
        return cleanValue.split('').join('-');
      }
    },
    methods:{
      addSeparator:function (event) {
        this.inputValue = event.target.value.replace(/-/g, '');
      }
    }
  }
</script>

<style scoped>
  input {
    padding: 6px 12px;
    outline: none;
    border-radius: 3px;
    border: 1px solid grey;
  }
</style>
