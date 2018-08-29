<template>
  <div id="app">
    <input v-model="inputValue"/>
    <button @click="handleSubmit">提交</button>
  </div>
</template>

<script>
export default {
  data () {
    return {
      inputValue: '',
      list: []
    }
  },
  methods: {
    handleSubmit: function () {
      this.list.push(this.inputValue)
    }
  }
}
</script>

<style>
</style>
